---
title: Item (UploadItemType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7058f2-615f-4393-a0d4-af76727f37e9
description: O elemento item representa um único item a ser carregado em uma caixa de correio.
ms.openlocfilehash: 82c0fdf89c06ddfb812c2b2f1899b589eedeb7d8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467547"
---
# <a name="item-uploaditemtype"></a>Item (UploadItemType)

O elemento **Item** representa um único item a ser carregado em uma caixa de correio. 
  
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
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**CreateAction** <br/> |Especifica a ação para carregar um item em uma caixa de correio. Esse atributo é necessário.  <br/> |
|**Isassociated** <br/> |Especifica se o item carregado é um item associado à pasta. Este atributo é um valor booliano. Um valor **true** indica que o item é um item associado à pasta. Esse atributo é opcional.  <br/> |
   
#### <a name="createaction-attribute"></a>Atributo CreateAction

|**Valor**|**Descrição**|
|:-----|:-----|
|**CreateNew** <br/> |Indica que uma nova cópia do item original é carregada na caixa de correio. O elemento [ItemId](itemid.md) não deve estar presente se o valor de CreateNew for usado. O novo identificador de item é retornado na resposta.  <br/> |
|**Atualização** <br/> |Especifica que o item indicado pelo elemento **ItemId** será atualizado. Um erro será retornado se o elemento **ItemId** não estiver presente ou se o item não existir na pasta identificada pelo elemento [ParentFolderId](parentfolderid.md) .  <br/> |
|**UpdateOrCreate** <br/> |Indica que uma tentativa é feita pela primeira vez para atualizar o item. Se o item não existir na pasta especificada pelo elemento **ParentFolderId** , um novo item é criado.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta pai onde um novo item é criado ou que contém o item a ser atualizado.  <br/> |
|[ItemId](itemid.md) <br/> |Contém o identificador exclusivo e a chave de alteração de um item a ser criado ou atualizado no repositório do Exchange.  <br/> |
|[Dados (base64Binary)](data-base64binary.md) <br/> |Contém os dados de um único item a ser carregado em uma caixa de correio.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Itens (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md) <br/> |Contém uma matriz de itens para carregar em uma caixa de correio.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação ExportItems](exportitems-operation.md)
  
[Operação UploadItems](uploaditems-operation.md)

