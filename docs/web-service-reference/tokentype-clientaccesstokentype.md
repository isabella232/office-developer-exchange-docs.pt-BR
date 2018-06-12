---
title: TokenType (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96103f15-a3e0-497c-af21-90adbf9a4b14
description: O elemento TokenType identifica o tipo de token de acesso de cliente que será retornado na resposta GetClientAccessToken.
ms.openlocfilehash: c9adb60acf76fefebd58e2fd3bc899332a63dbee
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837773"
---
# <a name="tokentype-clientaccesstokentype"></a>TokenType (ClientAccessTokenType)

O elemento **TokenType** identifica o tipo de token de acesso de cliente que será retornado na resposta **GetClientAccessToken** . 
  
```XML
<TokenType>CallerIdentity | ExtensionCallback | ScopedToken</TokenType>
```

 **ClientAccessTokenTypeType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[TokenRequest](tokenrequest.md) | [(ClientAccessTokenType) de Token](token-clientaccesstokentype.md)
  
## <a name="text-value"></a>Text value

Um valor de texto de **CallerIdentity** significa que um token de acesso de cliente de identidade de chamador será retornado. Um valor de texto de **ExtensionCallback** indica que um token de acesso de cliente de retorno de chamada de extensão será retornado. Um valor de texto de **ScopedToken** indica que o token de acesso do cliente é um token de escopo. 
  
## <a name="remarks"></a>Coment�rios

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |false  <br/> |
   

