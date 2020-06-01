---
title: RedirectTarget (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f8162724-cf9a-4543-a1ad-5846c8b10bfa
description: O elemento RedirectTarget (SOAP) contém o destino da URL de redirecionamento ou endereço de email.
ms.openlocfilehash: 092d575560379d43b12dd98a3efa155b59c31450
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462196"
---
# <a name="redirecttarget-soap"></a>RedirectTarget (SOAP)

O elemento [RedirectTarget (SOAP)](redirecttarget-soap.md) contém o destino da URL de redirecionamento ou endereço de email. 
  
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
|[Userresponse (SOAP)](userresponse-soap.md) <br/> |Representa uma resposta a uma solicitação GetUserSettings para um usuário individual.  <br/> |
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Contém as configurações solicitadas para o domínio especificado.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto contém o destino da URL de redirecionamento ou o endereço de email que deve ser usado para uma solicitação subsequente de GetUserSettings ou GetDomainSettings.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |messages. xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   

