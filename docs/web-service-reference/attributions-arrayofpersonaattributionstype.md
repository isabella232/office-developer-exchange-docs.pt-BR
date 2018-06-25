---
title: Atribuições (ArrayOfPersonaAttributionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f61d843c-bca5-4c88-9667-fd03d2a963a1
description: O elemento de atribuições Especifica uma matriz de informações de atribuição de um ou mais contatos ou destinatários do Active Directory agregados em que a pessoa associada.
ms.openlocfilehash: 52fecb4e4381d5e9dbbaf7134fa18068ba15f6ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751232"
---
# <a name="attributions-arrayofpersonaattributionstype"></a>Atribuições (ArrayOfPersonaAttributionsType)

O elemento de **atribuições** Especifica uma matriz de informações de atribuição de um ou mais contatos ou destinatários do Active Directory agregados em que a pessoa associada. 
  
```XML
<Attributions>
    <Attribution></Attribution>
</Attributions>
```

 **ArrayOfPersonaAttributionsType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Atribuição (PersonaAttributionType)](attribution-personaattributiontype.md) <br/> |Especifica uma instância em uma matriz de atributos de um elemento **PersonaType** .  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Pessoa](persona.md) <br/> |Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

