---
title: ExtractAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: bc213f0e-a655-44e9-9ac9-bc1673bae1fe
description: O elemento ExtractAllowed especifica se a extração de entidade está habilitada.
ms.openlocfilehash: a51adaba24ef6ee285acf786398d6e6cdfbfee35
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535323"
---
# <a name="extractallowed"></a>ExtractAllowed

O **elemento ExtractAllowed** especifica se a extração de entidade está habilitada. 
  
```XML
<ExtractAllowed>true | false</ExtractAllowed
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RightsManagementLicenseData](rightsmanagementlicensedata.md) <br/> |Especifica informações sobre a licença de gerenciamento de direitos.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** para o **elemento ExtractAllowed** indica que a extração de entidade está habilitada. Um valor **false** indica que a extração de entidade não está habilitada. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Tipo de esquema  <br/> |
|Arquivo de validação  <br/> |types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

