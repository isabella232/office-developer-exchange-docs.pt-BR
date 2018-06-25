---
title: Pessoas
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 65312428-548c-4fe9-971a-d0dab3be5ddf
description: O elemento de pessoas Especifica uma matriz de dados de pessoa retornados como o resultado de uma solicitação de FindPeople.
ms.openlocfilehash: df6f1af34872abe13a1d0f3a98b0354c55354e31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824712"
---
# <a name="people"></a>Pessoas

O elemento de **pessoas** Especifica uma matriz de dados de pessoa retornados como o resultado de uma solicitação de **FindPeople** . 
  
```XML
<People>
   <Persona/>
</People>
```

**ArrayOfPeopleType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

[Pessoa](persona.md)
  
### <a name="parent-elements"></a>Elementos pai

[FindPeopleResponse](findpeopleresponse.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

