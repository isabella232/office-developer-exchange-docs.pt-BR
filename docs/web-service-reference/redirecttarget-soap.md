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
description: O elemento RedirectTarget (SOAP) contém o destino do endereço de email ou a URL de redirecionamento.
ms.openlocfilehash: 3a8a0c39c6889730c9d17778c6a26f84fcbcd4a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825019"
---
# <a name="redirecttarget-soap"></a>RedirectTarget (SOAP)

O elemento [RedirectTarget (SOAP)](redirecttarget-soap.md) contém o destino do endereço de email ou a URL de redirecionamento. 
  
```XML
<RedirectTarget/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Resposta SOAP)](userresponse-soap.md) <br/> |Representa uma resposta a uma solicitação de GetUserSettings para um usuário individual.  <br/> |
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Contém as configurações solicitadas para o domínio especificado.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto contém o destino do redirecionamento URL ou endereço de email que deve ser usado para um GetUserSettings subsequentes ou GetDomainSettings solicitação.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   

