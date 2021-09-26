---
title: DeletedOccurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeletedOccurrence
api_type:
- schema
ms.assetid: ff24ea15-0cd7-407d-a378-73ec16451870
description: O elemento DeletedOccurrence representa uma ocorrência excluída de um item de calendário recorrente.
ms.openlocfilehash: 69e77f86097fe7037fc217806e4ef1b33b99c549
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542481"
---
# <a name="deletedoccurrence"></a>DeletedOccurrence

O **elemento DeletedOccurrence** representa uma ocorrência excluída de um item de calendário recorrente. 
  
```xml
<DeletedOccurrence>
   <Start/>
</DeletedOccurrence>
```

 **DeletedOccurrenceInfoType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
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
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)  
- [Referência do EWS para Exchange](ews-reference-for-exchange.md)

