---
title: TokenType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 83c650eb-7ab8-480c-a7c9-df60072ee042
description: O elemento TokenType especifica o tipo de token.
ms.openlocfilehash: a51ddfdd097a94370168077b9eca8be2e0581603
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523317"
---
# <a name="tokentype"></a>TokenType

O **elemento TokenType** especifica o tipo de token. 
  
```XML
<TokenType> CallerIdentity | ExtensionCallback | ScopedToken </TokenType>
```

 **ClientAccessTokenTypeType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[TokenRequest](tokenrequest.md)  |  [Token](token.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento TokenType** é o tipo de token. O valor de texto **de CallerIdentity** indica que o token é um token de identidade do chamador. O valor de texto **de ExtensionCallback** indica que o token é para um retorno de chamada de extensão. O valor de texto **de ScopedToken** indica que o token de acesso para cliente é um token com escopo. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |falso  <br/> |
   

