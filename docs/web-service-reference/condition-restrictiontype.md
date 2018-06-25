---
title: Condição (RestrictionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4fdb373e-bf1b-4cb0-bbfb-444c6c6cec50
description: O elemento de condição Especifica a condição que é usada para identificar o final de uma pesquisa para um FindItem ou uma operação FindConversation.
ms.openlocfilehash: 513fc21be52a90698f1c292d6d20d7cdaab07371
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751414"
---
# <a name="condition-restrictiontype"></a>Condição (RestrictionType)

O elemento de **condição** Especifica a condição que é usada para identificar o final de uma pesquisa para um **FindItem** ou uma operação **FindConversation** . 
  
```XML
<Condition>
    <SearchExpression></SearchExpression>
</Condition>
```

 **RestrictionType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SearchExpression](searchexpression.md) <br/> |Elemento abstrato que representa o elemento substituído dentro de uma restrição.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SeekToConditionPageItemView](seektoconditionpageitemview.md) <br/> |Identifica a condição que é usada para identificar o final de uma pesquisa, o índice inicial de uma pesquisa, as entradas máxima para retornar e as instruções de pesquisa para uma operação de **FindConversation** ou um **FindItem** .  <br/> |
   
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

