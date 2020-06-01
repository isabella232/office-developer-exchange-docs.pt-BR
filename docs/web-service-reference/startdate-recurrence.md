---
title: StartDate (recorrência)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartDate
api_type:
- schema
ms.assetid: bd65ac06-b3ac-4c9b-9568-3e4dc94378e7
description: O elemento StartDate representa a data de início de um item de calendário ou tarefa recorrente.
ms.openlocfilehash: 4514f126b1de31c64a2650b9e7cb6b7412a726c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457204"
---
# <a name="startdate-recurrence"></a>StartDate (recorrência)

O elemento **StartDate** representa a data de início de um item de calendário ou tarefa recorrente. 
  
```xml
<StartDate/>
```

**Date**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[EndDateRecurrence](enddaterecurrence.md) <br/> |Descreve a data de início e a data de término de um padrão de recorrência de item.  <br/> |
|[NoEndRecurrence](noendrecurrence.md) <br/> |Descreve a data de início de um padrão de recorrência de item que não tem uma data de término definida.  <br/> |
|[NumberedRecurrence](numberedrecurrence.md) <br/> |Descreve a data de início e o número de ocorrências de um item recorrente.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa uma data é necessário se esse elemento for usado. O valor não pode ser menor que abr, 1, 1601 00:00:00.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

