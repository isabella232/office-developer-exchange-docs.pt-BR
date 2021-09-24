---
title: Elementos XML de Descoberta Automática SOAP para Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: Encontre informações de referência do elemento XML para o serviço Web de Descoberta Automática SOAP Exchange.
ms.openlocfilehash: 5dcf4d6cd7a2b0b2987e59530dfbaae7b9993242
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539091"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a>Elementos XML de Descoberta Automática SOAP para Exchange 2013

Encontre informações de referência do elemento XML para o serviço Web de Descoberta Automática SOAP Exchange.
  
A documentação nesta seção se baseia nas instâncias do elemento XML de Descoberta Automática SOAP enviadas entre o cliente e o servidor. Esta documentação de instância XML baseia-se nos arquivos WSDL e de esquema localizados no diretório virtual que hospeda o serviço de Descoberta Automática SOAP. Os usuários autenticados podem navegar até o WSDL e arquivos de esquema usando uma URL semelhante a uma das seguintes:
  
- O local do arquivo WSDL: `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` ou `http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`
    
- O local do esquema de mensagens: `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` ou `http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd` 
    
O local do WSDL de Descoberta Automática SOAP e dos arquivos de esquema varia de acordo com a Exchange instalação.
  
O arquivo de esquema messages.xsd descreve os elementos XML que podem ser enviados em um header SOAP de Descoberta Automática e corpo SOAP. Este arquivo fornece um mapa geral do que a estrutura XML pode ser para uma determinada interação de mensagem de solicitação-resposta. A estrutura XML real que é enviada entre o cliente e o servidor baseia-se nas opções e no contexto no qual ela é usada. Os arquivos de esquema definem qual XML é possível. O intervalo real de XML que é enviado sobre o fio é baseado em qual operação é chamada, as informações solicitadas e as configurações do lado do servidor. 
  
## <a name="related-sections"></a>Seções relacionadas

- [Referência do serviço Web de Descoberta Automática SOAP para Exchange](soap-autodiscover-web-service-reference-for-exchange.md)    
- [Referência do EWS para Exchange](ews-reference-for-exchange.md)    
- [Referência do serviço Web de Unificação de Mensagens para Exchange](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a>Confira também

- [Referência do serviço Web de Descoberta Automática para Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Descoberta Automática do Exchange](../exchange-web-services/autodiscover-for-exchange.md)
- [Introdução ao uso dos serviços Web no Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

