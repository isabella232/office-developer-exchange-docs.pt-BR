---
title: Referência do serviço web POX descoberta automática do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: Encontre informações de referência para o serviço de descoberta automática de POX no Exchange.
ms.openlocfilehash: a8797fe714fd23049094c3ec2475b93fec4282c0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824867"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a>Referência do serviço web POX descoberta automática do Exchange

Encontre informações de referência para o serviço de descoberta automática de POX no Exchange.
  
O serviço de descoberta automática fornece as informações de configuração que o aplicativo usa para criar uma conexão a um servidor Exchange. Você pode usar o "XML sem formatação antigo" serviço de descoberta automática (POX) para enviar mensagens que consistem apenas das cargas XML, sem qualquer delimitadores envelopes SOAP, para localizar as configurações de um aplicativo cliente deve ter para se conectar ao Exchange.
  
> [!NOTE]
> Para clientes que têm como alvo versões do Exchange, começando com o Exchange Server 2010, recomendamos que você usa o serviço de descoberta automática do SOAP em vez do serviço de descoberta automática de POX. Clientes que visam o Exchange 2007 tem que usar o serviço Descoberta automática de POX. É recomendável que os clientes que usam o .NET Framework usam a API gerenciada de EWS, porque ele contém um cliente de descoberta automática de POX robusto e bem testado. Para obter mais informações sobre a API gerenciada de EWS, consulte [Introdução ao aplicativos cliente do EWS Managed API](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
Esta seção fornece informações sobre os elementos XML que são enviados entre o cliente e o servidor durante os redirecionamentos de solicitação de descoberta automática de POX e as configurações de usuário que são retornadas em uma resposta. A referência do elemento XML contém resumos dos quais representam os elementos e uma descrição das hierarquias de elemento potenciais que usam o elemento. Esta documentação aborda as instâncias XML que são enviadas entre o cliente e servidor. O serviço Descoberta automática de POX não tem um esquema explícito.
  
Os artigos nesta seção fornecem descrições das mensagens que são usadas para recuperar informações de configuração de descoberta automática usando o serviço de descoberta automática de POX e exemplos. 
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_InThisSection"> </a>

- [Solicitação de descoberta automática POX para Exchange](pox-autodiscover-request-for-exchange.md)
    
- [Resposta de descoberta automática POX para Exchange](pox-autodiscover-response-for-exchange.md)
    
- [Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a>Confira também

- [Referência de web service de descoberta automática do Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Descoberta Automática do Exchange](../exchange-web-services/autodiscover-for-exchange.md)   
- [SOAP referência de serviço web de descoberta automática do Exchange](soap-autodiscover-web-service-reference-for-exchange.md)
- [Start using web services in Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

