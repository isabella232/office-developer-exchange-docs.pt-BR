---
title: ImItemList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 556457d5-a730-4131-853f-1198c27c5942
description: O elemento ImItemList contém uma lista de grupos de mensagens instantâneas e contatos de mensagens instantâneas.
ms.openlocfilehash: fdd2865ceb1553a7f75d7059b08ea96ce89aa096
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547243"
---
# <a name="imitemlist"></a>ImItemList

O **elemento ImItemList** contém uma lista de grupos de mensagens instantâneas e contatos de mensagens instantâneas. 
  
```XML
<ImItemList>
   <Groups/>
   <Personas/>
</ImItemList>
```

 **ImItemListType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[Grupos (ArrayOfImGroupType)](groups-arrayofimgrouptype.md)  |  [Personas](personas-ex15websvcsotherref.md)
  
### <a name="parent-elements"></a>Elementos pai

[GetImItemsResponse](getimitemsresponse.md)  |  [GetImItemListResponse](getimitemlistresponse.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

