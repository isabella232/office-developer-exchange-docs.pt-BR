---
title: OldFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OldFolderId
api_type:
- schema
ms.assetid: da554a97-ab87-4950-9fc4-26b1972381bb
description: O elemento OldFolderId contém o identificador original de uma pasta que foi movido ou copiada.
ms.openlocfilehash: ef73cad73213a1e8b5341907cd22177d8e1ba628
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824645"
---
# <a name="oldfolderid"></a>OldFolderId

O elemento **OldFolderId** contém o identificador original de uma pasta que foi movido ou copiada. 
  
```xml
<OldFolderId Id="" ChangeKey=""/>
```

 **FolderIdType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**ID de** <br/> |Contém uma cadeia de caracteres que identifica uma pasta no repositório do Exchange. Este atributo é necessário.  <br/> |
|**ChangeKey** <br/> |Contém uma cadeia de caracteres que identifica uma versão de uma pasta que é identificada pelo atributo Id. Este atributo é opcional. Use este atributo para certificar-se de que a versão correta de uma pasta é usada.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CopiedEvent](copiedevent.md) <br/> |Representa um evento no qual uma pasta ou um item é copiada.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Representa um evento na qual um item ou pasta é movida de uma pasta pai para outra pasta pai.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Inscrever-se a operação](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
