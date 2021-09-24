---
title: DeleteFromFolderStateDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3aba59a0-f12a-48b5-842b-11cf4530dd51
description: O elemento DeleteFromFolderStateDefinition especifica o estado quando um item é excluído de uma pasta.
ms.openlocfilehash: 270edfc0b7abd70b74ff8c8b4353140ec5fbe27b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510236"
---
# <a name="deletefromfolderstatedefinition"></a>DeleteFromFolderStateDefinition

O **elemento DeleteFromFolderStateDefinition** especifica o estado quando um item é excluído de uma pasta. 
  
```XML
<DeleteFromFolderStateDefinition>
    <OccurrenceDate></OccurrenceDate>
    <IsOccurrencePresent></IsOccurrencePresent>
</DeleteFromFolderStateDefinition>
```

 **DeleteFromFolderStateDefinitionType**
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

