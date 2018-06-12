---
title: Elementos XML do EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exchange
api_type:
- schema
ms.assetid: 4653466a-a596-456f-bbff-7da4ef1d18d3
description: Encontre informações de referência para o XML EWS elementos no Exchange.
ms.openlocfilehash: 046a985ae4696616d28a0891ffe0aa8cc0552307
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752122"
---
# <a name="ews-xml-elements-in-exchange"></a>Elementos XML do EWS no Exchange

Encontre informações de referência para o XML EWS elementos no Exchange.
  
Serviços Web do Exchange (EWS) é um serviço web baseado em SOAP, o que significa que as mensagens de solicitação e resposta que são enviadas entre o cliente e servidor são compostas de elementos XML. A documentação desta seção baseia-se em instâncias XML que são enviadas entre o cliente e servidor. As instâncias XML são definidas nos arquivos de esquema e WSDL que estão localizados no diretório virtual que hospeda o EWS. Se você for um usuário autenticado, você pode navegar para os arquivos de esquema e WSDL usando as seguintes URLs, onde \<yourclientaccessserver\> é o nome do seu servidor de acesso para cliente:
  
- http://\<yourclientaccessserver\>.com/ews/services.wsdl — o local do arquivo WSDL.
    
- http://\<yourclientaccessserver\>.com/ews/messages.xsd — o local do esquema de mensagens.
    
- http://\<yourclientaccessserver\>.com/ews/types.xsd — o local do esquema tipos.
    
Os arquivos de esquema que descrevem os elementos XML do EWS fornecem um roteiro geral da estrutura XML que seja possível para interações de mensagem de solicitação de resposta. A estrutura XML real que é enviada entre cliente e servidor varia de acordo com a operação que é chamada, as informações solicitadas e as configurações do servidor.
  
O arquivo WSDL do EWS, services.wsdl, não totalmente acordo com o WSDL padrão porque ele não inclui uma definição de serviço WSDL. Isso ocorre porque o EWS não foi projetado para ser hospedados em um computador que tenha um endereço predefinido. Você pode usar o serviço Descoberta automática para obter o endereço do ponto de extremidade EWS. Alguns geradores de modelo de objeto do cliente analisar o WSDL e podem encontrar uma condição de erro porque o arquivo WSDL não contém uma definição de serviço WSDL. Se seu gerador de modelo de objeto encontra um erro, você pode inserir um espaço reservado para definição de WSDL do serviço.
  
> [!TIP]
> Se você estiver usando o .NET Framework para desenvolver seu aplicativo, é recomendável que você use a [API gerenciada de EWS](http://aka.ms/ews-managed-api-readme), em vez de um gerador de modelo de objeto. A API gerenciada de EWS fornece um modelo de objeto de fácil utilização para manipular a serialização e desserialização do EWS XML. Para obter mais informações, consulte [Introdução ao aplicativos cliente do EWS Managed API](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
O arquivo de esquema messages.xsd contém as definições de elemento para os elementos de nível superior no corpo SOAP. Com exceção dos códigos de resposta de erro, a maioria das definições em messages.xsd é específica para uma operação. O esquema de types.xsd contém as definições para os cabeçalhos SOAP e todas as definições comuns que são compartilhadas em operações.
  
## <a name="see-also"></a>Confira também

- [Referência do EWS para Exchange](ews-reference-for-exchange.md)
- [Operações do EWS no Exchange](ews-operations-in-exchange.md)
- [Explorar a API Gerenciada pelo EWS, EWS e serviços Web no Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Start using web services in Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Descoberta Automática do Exchange](../exchange-web-services/autodiscover-for-exchange.md)
    

