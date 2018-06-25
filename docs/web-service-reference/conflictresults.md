---
title: ConflictResults
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictResults
api_type:
- schema
ms.assetid: 08cdd547-4de7-4c7a-b60f-e618dc217d20
description: O elemento ConflictResults contém o número de conflitos em uma resposta de operação UpdateItem.
ms.openlocfilehash: faa6dc6c5fbbe874438a89c810a12fa675e8a1c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751425"
---
# <a name="conflictresults"></a>ConflictResults

O elemento [ConflictResults](conflictresults.md) contém o número de conflitos em uma resposta de [operação UpdateItem](updateitem-operation.md) . 
  
[UpdateItemResponse](updateitemresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[UpdateItemResponseMessage](updateitemresponsemessage.md)
  
[ConflictResults](conflictresults.md)
  
```xml
<ConflictResults>
   <Count/>
</ConflictResults>
```

 **ConflictResultsType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Count](count.md) <br/> |Contém o número de conflitos em uma resposta de [operação UpdateItem](updateitem-operation.md) .  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação UpdateItem](updateitem-operation.md) solicitação.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server com a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação UpdateItem](updateitem-operation.md)
  
 **ConflictResultsType**

