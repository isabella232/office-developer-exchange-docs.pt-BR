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
description: O elemento ItemChange contém um identificador de item e as atualizações a serem aplicadas ao item.
ms.openlocfilehash: 916ef1ba2c7a709ec1fd80ababd72999506773c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459914"
---
# <a name="itemchange"></a>ItemChange

O elemento **ItemChange** contém um identificador de item e as atualizações a serem aplicadas ao item. 
  
- [UpdateItem](updateitem.md) 
- [Alterações](itemchanges.md)
- [ItemChange](itemchange.md)
  
```xml
<ItemChange>
   <ItemId/>
   <Updates>...</Updates>
</ItemChange>
```

```xml
<ItemChange>
   <OccurrenceItemId>...</OccurrenceItemId>
   <Updates>...</Updates>
</ItemChange>
```

```xml
<ItemChange>
   <RecurringMasterItemId>...</RecurringMasterItemId>
   <Updates>...</Updates>
</ItemChange>
```

**Mychangtype**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange. Esse elemento é necessário se o elemento [OccurrenceItemId](occurrenceitemid.md) ou [RecurringMasterItemId](recurringmasteritemid.md) não é usado.  <br/> |
|[OccurrenceItemId](occurrenceitemid.md) <br/> |Identifica uma única ocorrência de um item recorrente. Este elemento será necessário se for usado. Este elemento é necessário se o elemento [RecurringMasterItemId](recurringmasteritemid.md) ou [ItemId](itemid.md) não é usado.  <br/> |
|[RecurringMasterItemId](recurringmasteritemid.md) <br/> |Identifica um item mestre de recorrência identificando um de seus identificadores de itens de ocorrência relacionados. Este elemento será necessário se for usado. Este elemento é necessário se o elemento [OccurrenceItemId](occurrenceitemid.md) ou [ItemId](itemid.md) não é usado.  <br/> |
|[Atualizações (item)](updates-item.md) <br/> |Contém uma matriz que define Append, set e Delete alterações nas propriedades do item. Este elemento é obrigatório.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Alterações](itemchanges.md) <br/> |Contém uma matriz de elementos [ItemChange](itemchange.md) que identificam itens e as atualizações a serem aplicadas aos itens.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/UpdateItem/ItemChanges` <br/> |
   
## <a name="remarks"></a>Comentários

Somente um único elemento [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md)ou [RecurringMasterItemId](recurringmasteritemid.md) pode ser usado em um elemento **ItemChange** . 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação UpdateItem](updateitem-operation.md)

