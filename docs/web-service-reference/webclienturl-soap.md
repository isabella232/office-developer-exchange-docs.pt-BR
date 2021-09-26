---
title: WebClientUrl (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 7f8cb6d6-4aac-4a1f-8bec-2dcb90fc1df6
description: O elemento WebClientUrl representa a URL de um cliente Exchange Web.
ms.openlocfilehash: 73cc03411e8356fafe078df45f9ebd695e8f154b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542593"
---
# <a name="webclienturl-soap"></a>WebClientUrl (SOAP)

O **elemento WebClientUrl** representa a URL de um cliente Exchange Web. 
  
[UserSetting (SOAP)](usersetting-soap.md)
  
[WebClientUrls (SOAP)](webclienturls-soap.md)
  
[WebClientUrl (SOAP)](webclienturl-soap.md)
  
```XML
<WebClientUrl>
    <AuthenticationMethods/>
    <Url/>
</WebClientUrl>
```

 **WebClientUrl**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AuthenticationMethods (SOAP)](authenticationmethods-soap.md) <br/> |Representa o método de autenticação a ser usado ao acessar a URL especificada.  <br/> |
|[Url (SOAP)](url-soap.md) <br/> |Representa o endereço da Web para a URL.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[WebClientUrls (SOAP)](webclienturls-soap.md) <br/> |Representa uma configuração de usuário que contém uma coleção de **elementos WebClientUrl.**  <br/> |
   
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Url (SOAP)](url-soap.md)
  
[WebClientUrls (SOAP)](webclienturls-soap.md)

