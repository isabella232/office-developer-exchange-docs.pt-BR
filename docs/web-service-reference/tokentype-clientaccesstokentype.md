---
title: TokenType (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 96103f15-a3e0-497c-af21-90adbf9a4b14
description: O elemento TokenType identifica o tipo de token de acesso para cliente que será retornado na resposta GetClientAccessToken.
ms.openlocfilehash: 967d64796799147876ef6443b40b16154b55c01a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523353"
---
# <a name="tokentype-clientaccesstokentype"></a>TokenType (ClientAccessTokenType)

O **elemento TokenType** identifica o tipo de token de acesso para cliente que será retornado na resposta **GetClientAccessToken.** 
  
```XML
<TokenType>CallerIdentity | ExtensionCallback | ScopedToken</TokenType>
```

 **ClientAccessTokenTypeType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[TokenRequest](tokenrequest.md)  |  [Token (ClientAccessTokenType)](token-clientaccesstokentype.md)
  
## <a name="text-value"></a>Valor de texto

Um valor de texto **de CallerIdentity significa** que um token de acesso para cliente de identidade de chamador é retornado. Um valor de texto **de ExtensionCallback** indica que um token de acesso para cliente de retorno de chamada de extensão é retornado. Um valor de texto **de ScopedToken** indica que o token de acesso para cliente é um token com escopo. 
  
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
   

