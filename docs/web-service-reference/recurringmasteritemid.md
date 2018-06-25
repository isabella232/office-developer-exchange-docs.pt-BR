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
description: O elemento RecurringMasterItemId identifica um item-mestre recorrência identificando os identificadores de um dos seus itens relacionados ocorrência.
ms.openlocfilehash: ae59e33ece55d85435ece4c9030ccda32eb62eab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825015"
---
# <a name="recurringmasteritemid"></a>RecurringMasterItemId

O elemento **RecurringMasterItemId** identifica um item-mestre recorrência identificando os identificadores de um dos seus itens relacionados ocorrência. 
  
```XML
<RecurringMasterItemId OccurrenceId="" ChangeKey="" />
```

 **RecurringMasterItemIdType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**OccurrenceId** <br/> |Identifica uma única ocorrência de um item mestre recorrente. Este atributo é necessário.  <br/> |
|**ChangeKey** <br/> |Identifica uma versão específica de uma única ocorrência de um item mestre recorrente. Além disso, o item mestre recorrente também é identificado porque ele e a ocorrência única irá conter a mesma chave de alteração. Este atributo é opcional.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |Contém o conjunto de identificadores de item para todos os itens de conversa em uma caixa de correio.  <br/> |
|[ItemChange](itemchange.md) <br/> |Contém um identificador de item e as atualizações para aplicar ao item. <br/> <br/> Este é a expressão XPath para esse elemento: <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[ItemIds](itemids.md) <br/> | Contém as identidades exclusivas dos itens, itens de ocorrência e itens recorrentes de mestres que são usados para excluir, enviar, obter, mover ou copiar itens no armazenamento do Exchange. <br/> <br/>  A seguir estão as expressões XPath para esse elemento:  <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="example"></a>Exemplo

O exemplo a seguir identifica o item mestre recorrente identificando um dos seus ocorrências com o identificador de 56lkjh6.
  
```XML
<RecurringMasterItemId OccurrenceId="56lkjh6" />
```

## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [OccurrenceItemId](occurrenceitemid.md)
- [Operação FindConversation](findconversation-operation.md)

