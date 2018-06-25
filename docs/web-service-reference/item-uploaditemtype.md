---
title: Item (UploadItemType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7058f2-615f-4393-a0d4-af76727f37e9
description: O elemento de Item representa um único item para carregar em uma caixa de correio.
ms.openlocfilehash: 8fecef9a2368a44e38633eb9fddaa8197620f6a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824138"
---
# <a name="item-uploaditemtype"></a>Item (UploadItemType)

O elemento de **Item** representa um único item para carregar em uma caixa de correio. 
  
[UploadItems](uploaditems.md)
  
[Itens (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md)
  
[Item (UploadItemType)](item-uploaditemtype.md)
  
```XML
<Item CreateAction="" IsAssociated="">
   <ParentFolderId/>
   <ItemId/>
   <Data/>
</Item>
```

 **UploadItemType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**CreateAction** <br/> |Especifica a ação para carregar um item em uma caixa de correio. Este atributo é necessário.  <br/> |
|**IsAssociated** <br/> |Especifica se o item carregado é um item de pasta associada. Este atributo é um valor booleano. Um valor **true** indica que o item é uma pasta associada item. Este atributo é opcional.  <br/> |
   
#### <a name="createaction-attribute"></a>Atributo CreateAction

|**Valor**|**Descrição**|
|:-----|:-----|
|**CreateNew** <br/> |Indica que uma nova cópia do item original é carregada na caixa de correio. O elemento [ItemId](itemid.md) não deve estar presente se o valor CreateNew é usado. O novo item identificador é retornado na resposta.  <br/> |
|**Update** <br/> |Especifica que o item indicado pelo elemento **ItemId** será atualizado. Um erro será retornado se o elemento **ItemId** não estiver presente ou se o item não existir na pasta identificada pelo elemento [ParentFolderId](parentfolderid.md) .  <br/> |
|**UpdateOrCreate** <br/> |Indica o primeiro é feita uma tentativa de atualizar o item. Se o item não existir na pasta especificada pelo elemento **ParentFolderId** , um novo item for criado.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta pai onde um novo item for criado ou que contém o item a ser atualizado.  <br/> |
|[ItemId](itemid.md) <br/> |Contém o identificador e alterar a chave exclusiva de um item para criar ou atualizar no armazenamento do Exchange.  <br/> |
|[Dados (base64Binary)](data-base64binary.md) <br/> |Contém os dados de um único item para carregar em uma caixa de correio.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Itens (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md) <br/> |Contém uma matriz de item para carregar em uma caixa de correio.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação ExportItems](exportitems-operation.md)
  
[Operação UploadItems](uploaditems-operation.md)

