---
title: CanRenameOrMove
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CanRenameOrMove
api_type:
- schema
ms.assetid: fe0cdb04-5f2b-4f1d-9d12-7ace0883cd86
description: O elemento CanRenameOrMove indica se uma pasta gerenciada pode ser renomeada ou movida pelo cliente.
ms.openlocfilehash: eb6aaeb8b0edcab5b67212c426a44daf32a0cf73
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463360"
---
# <a name="canrenameormove"></a>CanRenameOrMove

O elemento **CanRenameOrMove** indica se uma pasta gerenciada pode ser renomeada ou movida pelo cliente. 
  
```xml
<CanRenameOrMove/>
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
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |Contém informações sobre uma pasta gerenciada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa um valor booliano. Um valor **true** indica que a pasta pode ser renomeada ou movida; um valor **false** indica que a pasta não pode ser renomeada ou movida. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

