---
title: Elementos de Autodiscover XML SOAP para o Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: Encontre informações de referência de elemento XML para o serviço web de descoberta automática do SOAP no Exchange.
ms.openlocfilehash: 7201ef33060691df70b63d06b2045e1120b0610f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825517"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a>Elementos de Autodiscover XML SOAP para o Exchange 2013

Encontre informações de referência de elemento XML para o serviço web de descoberta automática do SOAP no Exchange.
  
A documentação desta seção se baseia nas instâncias de elemento XML de descoberta automática de SOAP que são enviadas entre o cliente e servidor. Esta documentação de instância XML baseia-se nos arquivos WSDL e do esquema que estão localizados no diretório virtual que hospeda o serviço de descoberta automática do SOAP. Usuários autenticados podem navegar para os arquivos de esquema e WSDL usando uma URL semelhante a um destes procedimentos:
  
- http://\<yourclientaccessserver\>.com/autodiscover/services.wsdl ou http://autodiscover.\<yourclientaccessserver\>.com/autodiscover/services.wsdl — o local do arquivo WSDL.
    
- http://\<yourclientaccessserver\>.com/autodiscover/messages.xsd ou http://autodiscover.\<yourclientaccessserver\>.com/autodiscover/messages.xsd — o local do esquema de mensagens.
    
O local dos arquivos de esquema e SOAP WSDL de descoberta automática varia de acordo com a instalação do Exchange.
  
O arquivo de esquema messages.xsd descreve os elementos XML que podem ser enviados em um cabeçalho SOAP de descoberta automática e o corpo SOAP. Este arquivo fornece um mapa geral dos quais a estrutura XML pode ser para uma interação de mensagem de solicitação-resposta determinado. A estrutura XML real que é enviada entre o cliente e o servidor se baseia nas opções e o contexto no qual ele é usado. Os arquivos de esquema definem o que é possível XML. O real intervalo de XML que será enviada pela conexão baseia-se na qual operação é chamado, as informações solicitadas e as configurações do servidor. 
  
## <a name="related-sections"></a>Se��es relacionadas
<a name="bk_RelatedSections"> </a>

- [SOAP referência de serviço web de descoberta automática do Exchange](soap-autodiscover-web-service-reference-for-exchange.md)
    
- [Referência do EWS para Exchange](ews-reference-for-exchange.md)
    
- [Referência de serviço de web mensagens unificada para Exchange](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a>Confira também

- [Referência de web service de descoberta automática do Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Descoberta Automática do Exchange](../exchange-web-services/autodiscover-for-exchange.md)
- [Start using web services in Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

