---
title: OccurrenceItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- OccurrenceItemId
api_type:
- schema
ms.assetid: 4a15bbc3-5b93-4193-b9ec-da32f0a9a552
description: O elemento OccurrenceItemId identifica uma única ocorrência de um item recorrente.
ms.openlocfilehash: ac6fc081e67f3897880ad30fcc1b62fe2e844459
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515414"
---
# <a name="occurrenceitemid"></a>OccurrenceItemId

O **elemento OccurrenceItemId** identifica uma única ocorrência de um item recorrente. 
  
```XML
<OccurrenceItemId RecurringMasterId="" ChangeKey="" InstanceIndex=""/>
```

**OccurrenceItemIdType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**RecurringMasterId** <br/> |Identifica o mestre recorrente de um item recorrente. Esse atributo é necessário.  <br/> |
|**ChangeKey** <br/> |Identifica uma versão específica do mestre recorrente ou uma ocorrência de item. Se o mestre recorrente ou qualquer uma de suas ocorrências mudar, **a ChangeKey** será mudada. O **ChangeKey** é o mesmo para o mestre recorrente e todas as ocorrências.  <br/> |
|**InstanceIndex** <br/> |Identifica o índice da ocorrência do item. Esse atributo é necessário. Esse valor representa um inteiro.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |Contém a coleção de identificadores de item para todos os itens de conversa em uma caixa de correio.  <br/> |
|[ItemIds](itemids.md) <br/> | Contém as identidades exclusivas de itens, itens de ocorrência e itens mestras recorrentes que são usados para excluir, enviar, obter, mover ou copiar itens no Exchange store. <br/><br/>Veja a seguir as expressões XPath para este elemento: <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/><br/>**OBSERVAÇÃO**: [a operação MoveItem e](moveitem-operation.md) a operação [CopyItem](copyitem-operation.md) funcionam apenas com itens de calendário único e itens mestras recorrentes. As ocorrências de item são inválidas com essas operações.           |
|[ItemChange](itemchange.md) <br/> |Contém um identificador de item e as atualizações a aplicar ao item.<br/><br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="example"></a>Exemplo

O exemplo a seguir identifica a quarta ocorrência de um item recorrente que tem a identidade 34vswe4.
  
```XML
<OccurrenceItemId RecurringMasterId="34vswe4" InstanceIndex="4" />
```

## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [RecurringMasterItemId](recurringmasteritemid.md)
- [Operação FindConversation](findconversation-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

