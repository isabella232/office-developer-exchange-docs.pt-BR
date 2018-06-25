---
title: DeletedOccurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeletedOccurrence
api_type:
- schema
ms.assetid: ff24ea15-0cd7-407d-a378-73ec16451870
description: O elemento DeletedOccurrence representa uma ocorrência excluída de um item de calendário recorrente.
ms.openlocfilehash: f12a2ba20f87f7803e492d8422b68c8ecdf9d797
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751736"
---
# <a name="deletedoccurrence"></a>DeletedOccurrence

O elemento **DeletedOccurrence** representa uma ocorrência excluída de um item de calendário recorrente. 
  
```xml
<DeletedOccurrence>
   <Start/>
</DeletedOccurrence>
```

 **DeletedOccurrenceInfoType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Start](start.md) <br/> |Representa a hora de início de uma ocorrência excluída de um item de calendário recorrente.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DeletedOccurrences](deletedoccurrences.md) <br/> |Contém uma matriz de ocorrências excluídas de um item de calendário recorrente.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)  
- [Referência do EWS para Exchange](ews-reference-for-exchange.md)

