---
title: DeletedOccurrenceStateDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: a9c01c64-e76c-4adc-8b04-88af97bd0cc8
description: A DeletedOccurrenceStateDefinition especifica o estado de uma ocorrência excluída de um item de calendário.
ms.openlocfilehash: 296eb1c99d5cc32cf8d1711bdb605ae10230ab34
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510278"
---
# <a name="deletedoccurrencestatedefinition"></a>DeletedOccurrenceStateDefinition

A **DeletedOccurrenceStateDefinition** especifica o estado de uma ocorrência excluída de um item de calendário. 
  
```XML
<DeletedOccurrenceStateDefinition>
    <OccurrenceDate></OccurrenceDate>
    <IsOccurrencePresent></IsOccurrencePresent>
</DeletedOccurrenceStateDefinition>
```

 **DeletedOccurrenceStateDefinitionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Occurrence (Time Zone Transition)](occurrence-time-zone-transition.md) <br/> |Especifica a data da ocorrência de um item de calendário.  <br/> |
|[IsOccurrencePresent](isoccurrencepresent.md) <br/> |Especifica um valor Boolean que indica se uma ocorrência do item de calendário está presente.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StateDefinition](statedefinition.md) <br/> |Especifica uma definição de estado.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Tipo de esquema  <br/> |
|Arquivo de validação  <br/> |types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

