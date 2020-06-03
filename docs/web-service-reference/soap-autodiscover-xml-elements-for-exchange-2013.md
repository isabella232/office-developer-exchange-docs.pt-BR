---
title: Elementos XML de descoberta automática SOAP para o Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: Encontre informações de referência do elemento XML para o serviço Web de descoberta automática SOAP no Exchange.
ms.openlocfilehash: 3b88429488dbecd4ed7c3adf56462f34fa0d4b17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465181"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a>Elementos XML de descoberta automática SOAP para o Exchange 2013

Encontre informações de referência do elemento XML para o serviço Web de descoberta automática SOAP no Exchange.
  
A documentação desta seção é baseada nas instâncias de elemento XML de descoberta automática do SOAP que são enviadas entre o cliente e o servidor. Esta documentação da instância XML baseia-se nos arquivos WSDL e de esquema localizados no diretório virtual que hospeda o serviço de descoberta automática do SOAP. Os usuários autenticados podem navegar para os arquivos WSDL e de esquema usando uma URL semelhante a uma das seguintes:
  
- O local do arquivo WSDL: `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` ou`http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`
    
- O local do esquema de mensagens: `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` ou`http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd` 
    
O local dos arquivos WSDL e do esquema de descoberta automática SOAP varia com base na instalação do Exchange.
  
O arquivo de esquema messages. xsd descreve os elementos XML que podem ser enviados em um cabeçalho SOAP de descoberta automática e no corpo SOAP. Este arquivo fornece um roteiro geral sobre o que a estrutura XML pode ser para uma determinada interação de mensagem de resposta de solicitação. A estrutura XML real que é enviada entre o cliente e o servidor baseia-se nas opções e no contexto em que é usada. Os arquivos de esquema definem o que é possível para o XML. O intervalo real de XML enviado pela conexão baseia-se na operação que é chamada, nas informações solicitadas e nas configurações do servidor. 
  
## <a name="related-sections"></a>Seções relacionadas

- [Referência de serviço Web de descoberta automática do SOAP para Exchange](soap-autodiscover-web-service-reference-for-exchange.md)    
- [Referência do EWS para Exchange](ews-reference-for-exchange.md)    
- [Referência do serviço Web de Unificação de mensagens do Exchange](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a>Confira também

- [Referência do serviço Web de descoberta automática do Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Descoberta Automática do Exchange](../exchange-web-services/autodiscover-for-exchange.md)
- [Introdução ao uso dos serviços Web no Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

