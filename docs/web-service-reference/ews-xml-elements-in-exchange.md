---
title: Elementos XML do EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- Exchange
api_type:
- schema
ms.assetid: 4653466a-a596-456f-bbff-7da4ef1d18d3
description: Encontre informações de referência para os elementos XML do EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: 29b90ad137141e30484ef804b6fcb6bb049ef3e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526113"
---
# <a name="ews-xml-elements-in-exchange"></a>Elementos XML do EWS no Exchange

Encontre informações de referência para os elementos XML do EWS no Exchange.
  
O EWS (serviços Web do Exchange) é um serviço Web baseado em SOAP, o que significa que as mensagens de solicitação e resposta enviadas entre o cliente e o servidor são compostas de elementos XML. A documentação desta seção é baseada nas instâncias XML que são enviadas entre o cliente e o servidor. As instâncias XML são definidas nos arquivos WSDL e de esquema que estão localizados no diretório virtual que hospeda o EWS. Se você for um usuário autenticado, poderá navegar até os arquivos WSDL e de esquema usando as seguintes URLs, onde \<yourclientaccessserver\> é o nome do servidor de acesso para cliente:
  
- http:// \<yourclientaccessserver\> . com/EWS/Services. WSDL — o local do arquivo WSDL.
    
- http:// \<yourclientaccessserver\> . com/EWS/messages. xsd — o local do esquema de mensagens.
    
- http:// \<yourclientaccessserver\> . com/EWS/Types. xsd — o local do esquema de tipos.
    
Os arquivos de esquema que descrevem os elementos XML do EWS fornecem um roteiro geral da estrutura XML que é possível para interações de mensagens de resposta de solicitação. A estrutura XML real que é enviada entre o cliente e o servidor varia de acordo com a operação que é chamada, as informações solicitadas e as configurações do lado do servidor.
  
O arquivo WSDL do EWS, Services. WSDL, não está totalmente em conformidade com o padrão WSDL porque não inclui uma definição de serviço WSDL. Isso ocorre porque o EWS não foi projetado para ser hospedado em um computador que tenha um endereço predefinido. Você pode usar o serviço de descoberta automática para obter o endereço do ponto de extremidade do EWS. Alguns geradores de modelos de objeto do lado do cliente analisam o WSDL e podem encontrar uma condição de erro porque o arquivo WSDL não contém uma definição de serviço WSDL. Se o gerador do modelo de objeto encontrar um erro, você pode inserir uma definição de serviço WSDL de espaço reservado.
  
> [!TIP]
> Se você estiver usando o .NET Framework para desenvolver seu aplicativo, recomendamos que você use a [API gerenciada do EWS](http://aka.ms/ews-managed-api-readme), em vez de um gerador de modelos de objeto. A API gerenciada do EWS fornece um modelo de objeto fácil de usar para lidar com a serialização e a desserialização do EWS XML. Para obter mais informações, consulte [introdução aos aplicativos clientes de API gerenciada do EWS](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
O arquivo de esquema messages. xsd contém as definições de elemento para os elementos de nível superior no corpo SOAP. Com exceção dos códigos de resposta de erro, a maioria das definições em messages. xsd são específicas para uma operação. O esquema Types. xsd contém as definições dos cabeçalhos SOAP e todas as definições comuns que são compartilhadas entre as operações.
  
## <a name="see-also"></a>Confira também

- [Referência do EWS para Exchange](ews-reference-for-exchange.md)
- [Operações do EWS no Exchange](ews-operations-in-exchange.md)
- [Explorar os recursos da API gerenciada por EWS, EWS e serviços Web no Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Introdução ao uso dos serviços Web no Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Descoberta Automática do Exchange](../exchange-web-services/autodiscover-for-exchange.md)
    

