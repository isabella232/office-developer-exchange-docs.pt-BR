---
title: Referência de web service de descoberta automática do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a01124a8-a8cf-4b80-8625-d7ee05690bca
description: Encontre conteúdo de referência para o serviço web de descoberta automática do Exchange.
ms.openlocfilehash: 48ca4a93c2120079cb675eabbc460bf0e75570b2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751242"
---
# <a name="autodiscover-web-service-reference-for-exchange"></a>Referência de web service de descoberta automática do Exchange

Encontre conteúdo de referência para o serviço web de descoberta automática do Exchange.
  
O serviço web de descoberta automática fornece as informações de configuração que o aplicativo usa para criar uma conexão a um servidor Exchange. Você pode usar uma das opções a seguir para se conectar a descoberta automática:
  
- Serviço de descoberta automática do SOAP — disponível aos clientes que se conectam ao versões do Exchange, começando com o Exchange 2010, incluindo o Exchange Online.
    
- "XML sem formatação antigo" serviço de descoberta automática de (POX) — disponível aos clientes que se conectam ao versões do Exchange, começando com o Exchange 2007, incluindo o Exchange Online. 
    
O SOAP e o serviço de descoberta automática de POX podem fornecer as informações de configuração que seu cliente usará para criar uma conexão a um servidor Exchange.
  
> [!NOTE]
> Para versões do Exchange, começando com o Exchange 2010, é recomendável que você usar o serviço de descoberta automática do SOAP em vez do serviço de descoberta automática de POX. O serviço de descoberta automática do SOAP fornece solicitações de configuração de descoberta automática em lote e controle mais específico sobre quais configurações são retornadas na resposta. 
  
Esta seção contém informações de referência para o serviço Descoberta automática do SOAP e o serviço de descoberta automática de POX.
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_InThisSection"> </a>

- [SOAP referência de serviço web de descoberta automática do Exchange](soap-autodiscover-web-service-reference-for-exchange.md)
    
- [Referência do serviço web POX descoberta automática do Exchange](pox-autodiscover-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a>Confira também

- [Referência de serviços Web do Exchange](web-services-reference-for-exchange.md)
- [Serviço de descoberta automática (SOAP)](http://msdn.microsoft.com/library/e24d1a1f-0d20-4bd9-ae4c-9112ecacea78%28Office.15%29.aspx)
- [Serviço de descoberta automática (POX)](http://msdn.microsoft.com/library/13c54de3-a91c-4424-8732-99dd8f2162ec%28Office.15%29.aspx)
    

