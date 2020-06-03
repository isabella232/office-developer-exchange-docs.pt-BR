---
title: Referência de serviço Web de descoberta automática do POX para o Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: Encontre informações de referência para o serviço de descoberta automática do POX no Exchange.
ms.openlocfilehash: 3c0ca368f4427be7759e2db58fb418b4822dea8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465650"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a>Referência de serviço Web de descoberta automática do POX para o Exchange

Encontre informações de referência para o serviço de descoberta automática do POX no Exchange.
  
O serviço de descoberta automática fornece as informações de configuração que o aplicativo usa para criar uma conexão com um servidor Exchange. Você pode usar o serviço de descoberta automática de "Plain Old XML" (POX) para enviar mensagens que consistam apenas de cargas XML, sem nenhum envelope SOAP delimitador, para localizar as configurações que um aplicativo cliente deve ter para se conectar ao Exchange.
  
> [!NOTE]
> Para clientes que direcionam versões do Exchange a partir do Exchange Server 2010, recomendamos que você use o serviço de descoberta automática SOAP em vez do serviço de descoberta automática do POX. Os clientes que direcionam o Exchange 2007 precisam usar o serviço de descoberta automática do POX. Recomendamos que os clientes que usam o .NET Framework usem a API gerenciada do EWS, pois ele contém um cliente de descoberta automática do POX e bem testado. Para obter mais informações sobre a API gerenciada do EWS, confira [introdução aos aplicativos clientes de API gerenciada do EWS](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
Esta seção fornece informações sobre os elementos XML que são enviados entre o cliente e o servidor durante o redirecionamento da solicitação de descoberta automática de POX e as configurações de usuário retornadas em uma resposta. A referência do elemento XML contém resumos dos elementos que representam e uma descrição das possíveis hierarquias de elemento que usam o elemento. Esta documentação abrange as instâncias XML que são enviadas entre o cliente e o servidor. O serviço de descoberta automática do POX não tem um esquema explícito.
  
Os artigos desta seção fornecem exemplos e descrições das mensagens usadas para recuperar as informações de configuração da descoberta automática usando o serviço de descoberta automática do POX. 
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_InThisSection"> </a>

- [Solicitação de descoberta automática do POX para o Exchange](pox-autodiscover-request-for-exchange.md)
    
- [Resposta de descoberta automática do POX para o Exchange](pox-autodiscover-response-for-exchange.md)
    
- [Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a>Confira também

- [Referência do serviço Web de descoberta automática do Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Descoberta Automática do Exchange](../exchange-web-services/autodiscover-for-exchange.md)   
- [Referência de serviço Web de descoberta automática do SOAP para Exchange](soap-autodiscover-web-service-reference-for-exchange.md)
- [Introdução ao uso dos serviços Web no Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

