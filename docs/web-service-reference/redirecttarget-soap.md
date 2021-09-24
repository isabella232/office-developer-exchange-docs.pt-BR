---
title: RedirectTarget (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: f8162724-cf9a-4543-a1ad-5846c8b10bfa
description: O elemento RedirectTarget (SOAP) contém o destino da URL de redirecionamento ou endereço de email.
ms.openlocfilehash: 0e09529f62dfde66f1ef05875bb0b0a0886db452
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513539"
---
# <a name="redirecttarget-soap"></a>RedirectTarget (SOAP)

O [elemento RedirectTarget (SOAP)](redirecttarget-soap.md) contém o destino da URL de redirecionamento ou endereço de email. 
  
```XML
<RedirectTarget/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UserResponse (SOAP)](userresponse-soap.md) <br/> |Representa uma resposta a uma solicitação GetUserSettings para um usuário individual.  <br/> |
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Contém as configurações solicitadas para o domínio especificado.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto contém o destino da URL de redirecionamento ou endereço de email que deve ser usado para uma solicitação GetUserSettings ou GetDomainSettings subsequente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   

