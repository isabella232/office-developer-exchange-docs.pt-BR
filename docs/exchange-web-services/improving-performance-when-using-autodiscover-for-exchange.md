---
title: Melhorar o desempenho ao usar a descoberta automática do Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: e65ff6b2-3810-43ad-9728-27308891b193
description: Aprenda sobre as maneiras de melhorar o desempenho do processo de descoberta automática no seu aplicativo.
ms.openlocfilehash: d9eef3bdc76c16cf92bdbb39b36be067f0c06215
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750888"
---
# <a name="improving-performance-when-using-autodiscover-for-exchange"></a>Melhorar o desempenho ao usar a descoberta automática do Exchange

Aprenda sobre as maneiras de melhorar o desempenho do processo de descoberta automática no seu aplicativo.
  
Há muitas razões para descoberta automática. Configurar seu aplicativo para se conectar ao Exchange sem intervenção do usuário é ótimo! Se você estiver lendo este artigo, você provavelmente já sabe todos os motivos para usar e adoro descoberta automática, para que nós não listá-las aqui. Em vez disso, vamos falar sobre uma possível desvantagem: desempenho.
  
Descoberta automática não é inerentemente um processo lento, mas não é inerentemente rápida ou. O [processo de descoberta automática](autodiscover-for-exchange.md) envolve muita atividade de rede e que apresenta muito potencial para atrasos. O processo de descoberta automática tem três fases; todos os três têm o potencial de afetar o desempenho: 
  
- Definir o grupo de candidatos de ponto de extremidade descoberta automática  para aplicativos executados em computadores do domínio, isso pode envolver [pesquisas de SCP](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md), que envolve a comunicação com os serviços de domínio Active Directory (AD DS).
    
- Tentar cada candidato  isso requer uma solicitação/resposta HTTP para cada ponto de extremidade do candidato.
    
- Tentar outras alternativas  quando os candidatos em seu pool de candidato de ponto de extremidade de descoberta automática não produzirem resultados, você pode fazer uma solicitação GET não autenticada (solicitação/resposta HTTP) e uma pesquisa de DNS.
    
Superficialmente isso pode não parecer muito. No entanto, imagine um cenário onde o pool de candidatos do ponto de extremidade de descoberta automática é mais de uma ou duas URLs, e você não encontrar um trabalho um até o último URL em seu pool. O atraso pode se tornar um pouco mais perceptível. Então, o que você pode fazer?
  
## <a name="consider-the-need-for-scp-lookup"></a>Considere a necessidade de pesquisa de SCP

Quando objetos SCP estão presentes e bem configuradas, elas podem acelerar o processo de descoberta automática. Em outras situações, no entanto, eles podem retardar a ele para baixo. Se o SCP não é usada no seu ambiente, pule a parte inteira de pesquisa SCP do processo de descoberta automática para economizar tempo.
  
A API gerenciada do EWS torna isso fácil: apenas definir a propriedade [ExchangeService.EnableScpLookup](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.enablescplookup%28v=exchg.80%29.aspx) de **false** antes de chamar o método [ExchangeService.AutodiscoverUrl](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) . Se você estiver usando a classe [AutodiscoverService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice%28v=exchg.80%29.aspx) , defina a propriedade de [AutodiscoverService.EnableScpLookup](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.enablescplookup%28v=exchg.80%29.aspx) de **false** antes de chamar qualquer um dos seus métodos. 
  
## <a name="use-autodiscover-less-often"></a>Usar descoberta automática menos freqüentemente

Descoberta automática não foi projetada para ser usado com freqüência usando aplicativos. O objetivo por trás da descoberta automática é um aplicativo para usá-lo para descobrir informações sobre a configuração e, em seguida, armazenar em cache essas informações por um período de tempo. Se você não armazenar em cache as informações de configuração, considere a adição de cache em seu aplicativo para reduzir o número de vezes que você usar descoberta automática.
  
Mesmo que você já está em cache, avalie quanto tempo você armazenar em cache as informações de configuração. O padrão é para [Atualizar informações de descoberta automática a cada 24 horas](how-to-refresh-configuration-information-by-using-autodiscover.md), mas você pode ser capaz de estender esse período. Você deve testar com os ambientes de destino e inventar um "time-to-live" para a configuração que funciona para você.
  
## <a name="minimize-requested-data"></a>Minimizar os dados solicitados

If you're using the **AutodiscoverService** class in the EWS Managed API, or the [Operação de GetUserSettings (SOAP)](http://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx) operation via SOAP, you have direct control over what settings are returned in the response. Although you can request quite a few settings, chances are that your application only needs a handful of them. Every setting that you request requires more processing on the server, which means more time waiting for a response. Evaluate the settings you are requesting, and eliminate any that you don't need. 
  
Se você estiver usando o método **ExchangeService.AutodiscoverUrl** na API gerenciada do EWS, você não pode alterar as configurações que você solicitar. No entanto, esse método já é bastante eficiente; Ele apenas solicita as configurações **ExternalEwsUrl** e **InternalEwsUrl** a [enumeração de UserSettingName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=exchg.80%29.aspx).
  
Se você estiver usando o serviço de descoberta automática de POX, [você não pode solicitar propriedades específicas](autodiscover-for-exchange.md#bk_Options).
  
## <a name="see-also"></a>Confira também


- [Descoberta Automática do Exchange](autodiscover-for-exchange.md)
    
- [Encontrar os pontos de extremidade de descoberta automática usando pesquisa do SCP no Exchange](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [Atualizar informações de configuração usando a descoberta automática](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [Classe ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)
    
- [Classe de AutodiscoverService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice%28v=exchg.80%29.aspx)
    

