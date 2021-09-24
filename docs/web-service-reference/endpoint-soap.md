---
title: Endpoint (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 630cdbb5-d1c7-422c-924a-abf5738e9e5e
description: O elemento Endpoint especifica o ponto de extremidade do serviço de token de segurança.
ms.openlocfilehash: 49a85dc80a92828262ab75652299d4a0c4d75de8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530970"
---
# <a name="endpoint-soap"></a>Endpoint (SOAP)

O **elemento Endpoint** especifica o ponto de extremidade do serviço de token de segurança. 
  
```XML
<Endpoint/>
```

 **xs:anyURI**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhuma
  
### <a name="child-elements"></a>Elementos filho

Nenhum
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[TokenIssuer (SOAP)](tokenissuer-soap.md) <br/> |Especifica o URI e o Ponto de Extremidade para o serviço de token de segurança.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o ponto de extremidade do serviço Web de token de segurança.
  
## <a name="remarks"></a>Comentários

O ponto de extremidade é usado para se comunicar com o serviço Web de token de segurança.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   

