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
ms.openlocfilehash: 3b88429488dbecd4ed7c3adf56462f34fa0d4b17
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353389"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a>Elementos de Autodiscover XML SOAP para o Exchange 2013

Encontre informações de referência de elemento XML para o serviço web de descoberta automática do SOAP no Exchange.
  
A documentação desta seção se baseia nas instâncias de elemento XML de descoberta automática de SOAP que são enviadas entre o cliente e servidor. Esta documentação de instância XML baseia-se nos arquivos WSDL e do esquema que estão localizados no diretório virtual que hospeda o serviço de descoberta automática do SOAP. Usuários autenticados podem navegar para os arquivos de esquema e WSDL usando uma URL semelhante a um destes procedimentos:
  
- O local do arquivo WSDL: `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` ou`http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`
    
- O local do esquema de mensagens: `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` ou`http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd` 
    
O local dos arquivos de esquema e SOAP WSDL de descoberta automática varia de acordo com a instalação do Exchange.
  
O arquivo de esquema messages.xsd descreve os elementos XML que podem ser enviados em um cabeçalho SOAP de descoberta automática e o corpo SOAP. Este arquivo fornece um mapa geral dos quais a estrutura XML pode ser para uma interação de mensagem de solicitação-resposta determinado. A estrutura XML real que é enviada entre o cliente e o servidor se baseia nas opções e o contexto no qual ele é usado. Os arquivos de esquema definem o que é possível XML. O real intervalo de XML que será enviada pela conexão baseia-se na qual operação é chamado, as informações solicitadas e as configurações do servidor. 
  
## <a name="related-sections"></a>Se��es relacionadas

- [SOAP referência de serviço web de descoberta automática do Exchange](soap-autodiscover-web-service-reference-for-exchange.md)    
- [Referência do EWS para Exchange](ews-reference-for-exchange.md)    
- [Referência de serviço de web mensagens unificada para Exchange](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a>Confira também

- [Referência de web service de descoberta automática do Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Descoberta Automática do Exchange](../exchange-web-services/autodiscover-for-exchange.md)
- [Start using web services in Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

