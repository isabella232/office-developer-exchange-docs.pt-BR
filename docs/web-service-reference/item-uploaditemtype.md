---
title: Item (UploadItemType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ab7058f2-615f-4393-a0d4-af76727f37e9
description: O elemento Item representa um único item a ser carregado em uma caixa de correio.
ms.openlocfilehash: bd4681a19df2018db9e54ee39095cd602662650a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514442"
---
# <a name="item-uploaditemtype"></a>Item (UploadItemType)

O **elemento Item** representa um único item a ser carregado em uma caixa de correio. 
  
[UploadItems](uploaditems.md)
  
[Items (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md)
  
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
|**IsAssociated** <br/> |Especifica se o item carregado é um item associado à pasta. Esse atributo é um valor Boolean. Um valor **true** indica que o item é um item associado à pasta. Esse atributo é opcional.  <br/> |
   
#### <a name="createaction-attribute"></a>Atributo CreateAction

|**Valor**|**Descrição**|
|:-----|:-----|
|**CreateNew** <br/> |Indica que uma nova cópia do item original é carregada na caixa de correio. O [elemento ItemId](itemid.md) não deve estar presente se o valor CreateNew for usado. O novo identificador de item é retornado na resposta.  <br/> |
|**Atualização** <br/> |Especifica que o item indicado pelo **elemento ItemId** será atualizado. Um erro será retornado se o **elemento ItemId** não estiver presente ou se o item não existir na pasta identificada pelo [elemento ParentFolderId.](parentfolderid.md)  <br/> |
|**UpdateOrCreate** <br/> |Indica que uma tentativa é feita pela primeira vez para atualizar o item. Se o item não existir na pasta especificada pelo **elemento ParentFolderId,** um novo item será criado.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta pai onde um novo item é criado ou que contém o item a ser atualizado.  <br/> |
|[ItemId](itemid.md) <br/> |Contém o identificador exclusivo e a chave de alteração de um item para criar ou atualizar no Exchange store.  <br/> |
|[Data (base64Binary)](data-base64binary.md) <br/> |Contém os dados de um único item a ser carregado em uma caixa de correio.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Items (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md) <br/> |Contém uma matriz de item a ser carregada em uma caixa de correio.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services. Esse elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação ExportItems](exportitems-operation.md)
  
[Operação UploadItems](uploaditems-operation.md)

