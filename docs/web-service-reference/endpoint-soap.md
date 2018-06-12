---
title: Ponto de extremidade (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 630cdbb5-d1c7-422c-924a-abf5738e9e5e
description: O elemento de ponto de extremidade Especifica o ponto de extremidade de serviço de token de segurança.
ms.openlocfilehash: 85e1ad785b35649238ac3944f51472addf617c20
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752063"
---
# <a name="endpoint-soap"></a>Ponto de extremidade (SOAP)

O elemento de **ponto de extremidade** Especifica o ponto de extremidade de serviço de token de segurança. 
  
```XML
<Endpoint/>
```

 **xs: anyURI**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhuma
  
### <a name="child-elements"></a>Elementos filho

None
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[TokenIssuer (SOAP)](tokenissuer-soap.md) <br/> |Especifica o URI e o ponto de extremidade para o serviço de token de segurança.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa o ponto de extremidade para o serviço web de token de segurança.
  
## <a name="remarks"></a>Coment�rios

O ponto de extremidade é usado para comunicação com o serviço web de token de segurança.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   

