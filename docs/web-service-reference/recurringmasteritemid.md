---
title: RecurringMasterItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringMasterItemId
api_type:
- schema
ms.assetid: 5800b58c-f3d7-4d8f-acc0-d13e02f4e258
description: O elemento RecurringMasterItemId identifica um item mestre de recorrência identificando os identificadores de um de seus itens de ocorrência relacionados.
ms.openlocfilehash: 896a9ce95d619e7bb44c8158288bc4f62ce417d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529879"
---
# <a name="recurringmasteritemid"></a>RecurringMasterItemId

O elemento **RecurringMasterItemId** identifica um item mestre de recorrência identificando os identificadores de um de seus itens de ocorrência relacionados. 
  
```XML
<RecurringMasterItemId OccurrenceId="" ChangeKey="" />
```

 **RecurringMasterItemIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Occurrences** <br/> |Identifica uma única ocorrência de um item mestre recorrente. Esse atributo é necessário.  <br/> |
|**ChangeKey** <br/> |Identifica uma versão específica de uma única ocorrência de um item mestre recorrente. Além disso, o item mestre recorrente também é identificado porque ele e a ocorrência única conterá a mesma chave de alteração. Esse atributo é opcional.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |Contém a coleção de identificadores de item para todos os itens de conversa em uma caixa de correio.  <br/> |
|[ItemChange](itemchange.md) <br/> |Contém um identificador de item e as atualizações a serem aplicadas ao item. <br/> <br/> A seguir está a expressão XPath para este elemento: <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[ItemIds](itemids.md) <br/> | Contém as identidades exclusivas de itens, itens de ocorrência e itens mestre recorrentes que são usados para excluir, enviar, obter, mover ou copiar itens no repositório do Exchange. <br/> <br/>  A seguir estão as expressões XPath para este elemento:  <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="example"></a>Exemplo

O exemplo a seguir identifica o item mestre recorrente identificando uma de suas ocorrências com o identificador 56lkjh6.
  
```XML
<RecurringMasterItemId OccurrenceId="56lkjh6" />
```

## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [OccurrenceItemId](occurrenceitemid.md)
- [Operação FindConversation](findconversation-operation.md)

