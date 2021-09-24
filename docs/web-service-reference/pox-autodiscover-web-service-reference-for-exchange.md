---
title: Referência do serviço Web de Descoberta Automática POX para Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: Encontre informações de referência para o serviço de Descoberta Automática POX Exchange.
ms.openlocfilehash: b28ea64a82960a84dee06c5055ee915614f4fde7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516416"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a>Referência do serviço Web de Descoberta Automática POX para Exchange

Encontre informações de referência para o serviço de Descoberta Automática POX Exchange.
  
O serviço descoberta automática fornece as informações de configuração que seu aplicativo usa para criar uma conexão com um Exchange servidor. Você pode usar o serviço de Descoberta Automática "XML antigo" (POX) para enviar mensagens que consistem apenas em cargas XML, sem nenhum envelope SOAP incluído, para localizar as configurações que um aplicativo cliente deve ter para se conectar ao Exchange.
  
> [!NOTE]
> Para clientes que direcionam versões de Exchange a partir do Exchange Server 2010, recomendamos que você use o serviço soap Descoberta Automática em vez do serviço de Descoberta Automática POX. Os clientes destinados Exchange 2007 têm que usar o serviço de Descoberta Automática POX. Recomendamos que os clientes que usam o .NET Framework usem a API Gerenciada do EWS porque ela contém um cliente de Descoberta Automática POX robusto e bem testado. Para obter mais informações sobre a API Gerenciada do EWS, consulte [Get started with EWS Managed API client applications](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
Esta seção fornece informações sobre os elementos XML que são enviados entre o cliente e o servidor durante redirecionamentos de solicitação de Descoberta Automática POX e as configurações do usuário que são retornadas em uma resposta. A referência do elemento XML contém resumos do que os elementos representam e uma descrição das hierarquias de elemento potencial que usam o elemento. Esta documentação abrange as instâncias XML enviadas entre o cliente e o servidor. O serviço de Descoberta Automática POX não tem um esquema explícito.
  
Os artigos nesta seção fornecem exemplos e descrições das mensagens usadas para recuperar informações de configuração de Descoberta Automática usando o serviço de Descoberta Automática POX. 
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_InThisSection"> </a>

- [Solicitação de Descoberta Automática POX para Exchange](pox-autodiscover-request-for-exchange.md)
    
- [Resposta de Descoberta Automática POX para Exchange](pox-autodiscover-response-for-exchange.md)
    
- [Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a>Confira também

- [Referência do serviço Web de Descoberta Automática para Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Descoberta Automática do Exchange](../exchange-web-services/autodiscover-for-exchange.md)   
- [Referência do serviço Web de Descoberta Automática SOAP para Exchange](soap-autodiscover-web-service-reference-for-exchange.md)
- [Introdução ao uso dos serviços Web no Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

