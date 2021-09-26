---
title: TargetAutodiscoverEpr (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: fdb9cc7a-cf0a-431b-9f6f-5f1db1792db7
description: O elemento TargetAutodiscoverEpr representa a propriedade TargetAutodiscoverEpr. O elemento TargetAutodiscoverEpr é apenas para uso interno. Esse elemento não é usado pelos clientes.
ms.openlocfilehash: f49d7b0acc59d638f2fca993ec7d8f182cd7380a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545801"
---
# <a name="targetautodiscoverepr-soap"></a>TargetAutodiscoverEpr (SOAP)

O **elemento TargetAutodiscoverEpr** representa a **propriedade TargetAutodiscoverEpr.** O **elemento TargetAutodiscoverEpr** é apenas para uso interno. Esse elemento não é usado pelos clientes. 
  
```XML
<TargetAutodiscoverEpr/>
```

 **anyURI**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Representa uma lista de relações de organização para uma única organização.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto para esse elemento é um URI (identificador de recurso uniforme) para a relação da organização.
  
## <a name="remarks"></a>Comentários

Esse elemento especifica a URL de Descoberta Automática do servidor para a organização externa. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

