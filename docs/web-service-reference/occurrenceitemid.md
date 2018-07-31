---
title: OccurrenceItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OccurrenceItemId
api_type:
- schema
ms.assetid: 4a15bbc3-5b93-4193-b9ec-da32f0a9a552
description: O elemento OccurrenceItemId identifica uma única ocorrência de um item recorrente.
ms.openlocfilehash: 073639ecbca6ffda872e9253b7c7e44c3541f13b
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353459"
---
# <a name="occurrenceitemid"></a>OccurrenceItemId

O elemento **OccurrenceItemId** identifica uma única ocorrência de um item recorrente. 
  
```XML
<OccurrenceItemId RecurringMasterId="" ChangeKey="" InstanceIndex=""/>
```

**OccurrenceItemIdType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**RecurringMasterId** <br/> |Identifica o mestre recorrente de um item recorrente. Este atributo é necessário.  <br/> |
|**ChangeKey** <br/> |Identifica uma versão específica do mestre recorrente ou uma ocorrência de item. Se o mestre recorrente ou qualquer um dos seus ocorrências alterar, altera a **ChangeKey** . A **ChangeKey** é a mesma para o mestre recorrente e todas as ocorrências.  <br/> |
|**InstanceIndex** <br/> |Identifica o índice da ocorrência item. Este atributo é necessário. Esse valor representa um número inteiro.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |Contém o conjunto de identificadores de item para todos os itens de conversa em uma caixa de correio.  <br/> |
|[ItemIds](itemids.md) <br/> | Contém as identidades exclusivas dos itens, itens de ocorrência e itens recorrentes de mestres que são usados para excluir, enviar, obter, mover ou copiar itens no armazenamento do Exchange. <br/><br/>A seguir estão as expressões XPath para esse elemento: <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/><br/>**Observação**: [operação MoveItem](moveitem-operation.md) e [operação CopyItem](copyitem-operation.md) só funcionam com itens de calendário único e itens recorrentes de mestres. Ocorrências de item são inválidas com essas operações.           |
|[ItemChange](itemchange.md) <br/> |Contém um identificador de item e as atualizações para aplicar ao item.<br/><br/> Este é a expressão XPath para esse elemento:  <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="example"></a>Exemplo

O exemplo a seguir identifica a quarta ocorrência de um item recorrente que tem o 34vswe4 de identidade.
  
```XML
<OccurrenceItemId RecurringMasterId="34vswe4" InstanceIndex="4" />
```

## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [RecurringMasterItemId](recurringmasteritemid.md)
- [Operação FindConversation](findconversation-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

