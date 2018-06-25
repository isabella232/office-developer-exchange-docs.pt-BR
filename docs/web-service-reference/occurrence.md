---
title: Ocorrência
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Occurrence
api_type:
- schema
ms.assetid: d292b99c-b896-40b7-be5d-2cb314c9481f
description: O elemento de ocorrência representa uma única ocorrência de modificação de um item de calendário recorrente.
ms.openlocfilehash: 5a40faa9b885a235d30e7f41830d1eefe2ed23c3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824653"
---
# <a name="occurrence"></a>Ocorrência

O elemento de **ocorrência** representa uma única ocorrência de modificação de um item de calendário recorrente. 
  
```xml
<Occurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</Occurrence>
```

**OccurrenceInfoType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |Contém a chave exclusiva de identificador e alteração de uma ocorrência modificada de um item de calendário recorrente.  <br/> |
|[Start](start.md) <br/> |Representa a hora de início de uma ocorrência modificada de um item de calendário recorrente.  <br/> |
|[End](end-ex15websvcsotherref.md) <br/> |Representa a hora de término de uma ocorrência modificada de um item de calendário recorrente.  <br/> |
|[OriginalStart](originalstart.md) <br/> |Representa a hora de início original de um item de calendário recorrente a uma ocorrência modificada.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ModifiedOccurrences](modifiedoccurrences.md) <br/> |Contém uma coleção de recorrente ocorrências de item de calendário que foram modificados para que sejam diferentes do que o item de recorrência mestre.  <br/> |
   
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

