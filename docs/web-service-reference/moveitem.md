---
title: MoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MoveItem
api_type:
- schema
ms.assetid: a4593377-22dd-415f-b01d-387389ef650f
description: O elemento MoveItem define uma solicitação para mover um item no Exchange store.
ms.openlocfilehash: 5df569722534b8a248da64b71f21219866173aab
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509599"
---
# <a name="moveitem"></a>MoveItem

O **elemento MoveItem** define uma solicitação para mover um item no Exchange store. 
  
```XML
<MoveItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</MoveItem>
```

 **MoveItemType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ToFolderId](tofolderid.md) <br/> |Representa a pasta de destino de um item movido.  <br/> |
|[ItemIds](itemids.md) <br/> |Contém uma matriz de itens identificados para mover para a pasta representada pelo [elemento ToFolderId.](tofolderid.md)  <br/> |
|[ReturnNewItemIds](returnnewitemids.md) <br/> |Indica se os identificadores de item de novos itens são retornados na resposta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação MoveItem](moveitem-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

