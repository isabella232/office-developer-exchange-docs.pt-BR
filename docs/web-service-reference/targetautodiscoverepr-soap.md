---
title: TargetAutodiscoverEpr (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: fdb9cc7a-cf0a-431b-9f6f-5f1db1792db7
description: O elemento TargetAutodiscoverEpr representa a propriedade TargetAutodiscoverEpr. O elemento TargetAutodiscoverEpr é apenas para uso interno. Este elemento não é usado pelos clientes.
ms.openlocfilehash: 0b28444727e21a98925b6d1062bcbbac62c68981
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837694"
---
# <a name="targetautodiscoverepr-soap"></a>TargetAutodiscoverEpr (SOAP)

O elemento **TargetAutodiscoverEpr** representa a propriedade **TargetAutodiscoverEpr** . O elemento **TargetAutodiscoverEpr** é apenas para uso interno. Este elemento não é usado pelos clientes. 
  
```XML
<TargetAutodiscoverEpr/>
```

 **anyURI**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Representa uma lista de relacionamentos de organização para uma única organização.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto para esse elemento é um identificador de recurso uniforme (URI) para o relacionamento da organização.
  
## <a name="remarks"></a>Coment�rios

Este elemento Especifica a URL de descoberta automática do servidor para a organização externa. 
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação de GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

