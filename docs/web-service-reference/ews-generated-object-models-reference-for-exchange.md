---
title: Modelos de objeto do Exchange gerados pelos Serviços Web do Exchange (EWS)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 67d7d831-9c53-46da-80e4-18f562e71284
description: Se você estiver usando a referência de modelos de objeto gerados pelos EWS para desenvolver aplicativos para o Exchange, saiba mais sobre outras opções para o desenvolvimento nos EWS.
ms.openlocfilehash: 6c97ca7973da84d96d102287b9c260409a0f57ef
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541431"
---
# <a name="ews-generated-object-models-for-exchange"></a>Modelos de objeto do Exchange gerados pelos EWS

**Aplica-se a**: Exchange Online | Exchange Server 2013 | Office 365

Inicialmente, o modelo de objeto dos Serviços Web do Exchange (EWS) gerados por wsdl.exe forneciam um modelo de objeto conveniente para trabalhar com o Exchange 2007. No entanto, quando a API gerenciada pelos EWS foi disponibilizada, introduziu várias vantagens para desenvolvedores que trabalham com código gerenciado. 

A API gerenciada do EWS:

- Fornece um modelo de objeto mais intuitivo.

- Contém lógica de negócios e validação de dados do lado do cliente.

- É totalmente compatível e atualizado regularmente.

- Contém um cliente de Descoberta Automática.

- Implementa recursos cliente, como login, gerenciamento de cookies e relatórios de diagnóstico, de volta para o Exchange.

A documentação de referência gerenciada baseada em wsdl.exe dos EWS foi removida, porque a API gerenciada pelos EWS substitui a maior parte da funcionalidade fornecida pelos modelos de objeto gerados. Ao mesmo tempo, sabemos que a API gerenciada pelos EWS não serve para todos. Na maioria das vezes, é a melhor maneira de criar clientes EWS para .NET, mas há algumas exceções, por exemplo:

- Talvez você queira usar uma funcionalidade que [não foi implementada na API gerenciada pelos EWS](../exchange-web-services/web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md#bk_apifeatures).

- Quando você está usando uma plataforma de desenvolvimento que não é a .NET.

Se não for possível usar a API gerenciada pelos EWS para desenvolver seu aplicativo, você poderá:

- Usar uma API cliente dos EWS terceirizada.

- Criar seu próprio modelo de objeto do cliente dos EWS.

- Usar um gerador de modelos de objeto. Você encontrará geradores de modelos de objeto compatíveis com a maioria das principais plataformas e linguagens.

Caso pretenda usar um gerador de modelos de objeto, você poderá usar a referência XML para entender o modelo de objeto gerado. O modelo de objeto é gerado a partir das estruturas XML descritas no esquema. Normalmente, as classes criadas por geradores de modelos de objeto mapeiam para tipos complexos no esquema. Propriedades que normalmente mapeiam para os elementos XML.

Confira o [Namespace ExchangeWebServices](https://docs.microsoft.com/dotnet/api/exchangewebservices?view=exchange-ews-proxy).

## <a name="see-also"></a>Confira também

- [Referência de serviço Web do Exchange](web-services-reference-for-exchange.md)
- [Explorar os recursos da API gerenciada por EWS, EWS e serviços Web no Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Novidades no EWS e outros serviços Web no Exchange](../exchange-web-services/whats-new-in-ews-and-other-web-services-in-exchange.md)
