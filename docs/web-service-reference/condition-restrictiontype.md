---
title: Condition (RestrictionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 4fdb373e-bf1b-4cb0-bbfb-444c6c6cec50
description: O elemento Condition especifica a condição usada para identificar o final de uma pesquisa para um FindItem ou uma operação FindConversation.
ms.openlocfilehash: f6292d2d25b9d236d0bb611c41a4cfcf490b6df4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543524"
---
# <a name="condition-restrictiontype"></a>Condition (RestrictionType)

O **elemento Condition** especifica a condição usada para identificar o final de uma pesquisa para um **FindItem** ou uma **operação FindConversation.** 
  
```XML
<Condition>
    <SearchExpression></SearchExpression>
</Condition>
```

 **RestrictionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SearchExpression](searchexpression.md) <br/> |Elemento abstrato que representa o elemento substituído dentro de uma restrição.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SeekToConditionPageItemView](seektoconditionpageitemview.md) <br/> |Identifica a condição usada para identificar o final de uma pesquisa, o índice inicial de uma pesquisa, as entradas máximas a retornar e as instruções de pesquisa para uma **operação FindItem** ou **FindConversation.**  <br/> |
   
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

