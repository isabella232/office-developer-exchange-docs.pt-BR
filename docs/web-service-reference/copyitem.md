---
title: CopyItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CopyItem
api_type:
- schema
ms.assetid: ffb4c13e-e7ea-4e6b-87a0-509ce5371100
description: O elemento CopyItem define uma solicitação para copiar um item em uma caixa de correio no Exchange store.
ms.openlocfilehash: 7f083f09a587b4788180711039e1cfdbbe6a10cd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529173"
---
# <a name="copyitem"></a>CopyItem

O **elemento CopyItem** define uma solicitação para copiar um item em uma caixa de correio no Exchange store. 
  
```XML
<CopyItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</CopyItem>
```

 **CopyItemType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ToFolderId](tofolderid.md) <br/> |Representa a pasta de destino de um item copiado.  <br/> |
|[ItemIds](itemids.md) <br/> |Contém uma matriz de itens identificados para copiar para a pasta representada pelo [elemento ToFolderId.](tofolderid.md)  <br/> |
|[ReturnNewItemIds](returnnewitemids.md) <br/> |Indica se os identificadores de item de novos itens são retornados na resposta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

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



[Operação CopyItem](copyitem-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

