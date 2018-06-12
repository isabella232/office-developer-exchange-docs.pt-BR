---
title: ItemChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemChange
api_type:
- schema
ms.assetid: 5cb43b02-d444-4d9c-9075-cdc5a4427daf
description: O elemento ItemChange contém um identificador de item e as atualizações para aplicar ao item.
ms.openlocfilehash: d10ce96cacb0be7411c4e8230ebc9b2803b7a5b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824145"
---
# <a name="itemchange"></a>ItemChange

O elemento **ItemChange** contém um identificador de item e as atualizações para aplicar ao item. 
  
[UpdateItem](updateitem.md)
  
[ItemChanges](itemchanges.md)
  
[ItemChange](itemchange.md)
  
```xml
<ItemChange>
   <ItemId/>
   <Updates>...</Updates>
</ItemChange>
```

 **ItemChangeType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |Contém o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange. Esse elemento é necessário se o elemento [OccurrenceItemId](occurrenceitemid.md) ou [RecurringMasterItemId](recurringmasteritemid.md) não for usado.  <br/> |
|[OccurrenceItemId](occurrenceitemid.md) <br/> |Identifica uma única ocorrência de um item recorrente. Esse elemento é obrigatório se usada. Esse elemento é necessário se o elemento [RecurringMasterItemId](recurringmasteritemid.md) ou [ItemId](itemid.md) não for usado.  <br/> |
|[RecurringMasterItemId](recurringmasteritemid.md) <br/> |Identifica um item-mestre recorrência identificando um dos identificadores dos seus itens relacionados ocorrência. Esse elemento é obrigatório se usada. Esse elemento é necessário se o elemento [OccurrenceItemId](occurrenceitemid.md) ou [ItemId](itemid.md) não for usado.  <br/> |
|[Atualizações (Item)](updates-item.md) <br/> |Contém uma matriz que define append, definir e excluir as alterações nas propriedades do item. Este elemento é obrigatório.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemChanges](itemchanges.md) <br/> |Contém uma matriz de elementos [ItemChange](itemchange.md) que identificam os itens e as atualizações para aplicar aos itens.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/UpdateItem/ItemChanges` <br/> |
   
## <a name="remarks"></a>Coment�rios

Somente um único elemento de [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md)ou [RecurringMasterItemId](recurringmasteritemid.md) pode ser usado em um elemento **ItemChange** . 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação UpdateItem](updateitem-operation.md)

