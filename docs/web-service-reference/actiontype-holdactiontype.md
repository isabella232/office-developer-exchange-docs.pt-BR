---
title: ActionType (HoldActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f50449b9-e73b-43c5-af96-6433bf434dce
description: O elemento ActionType indica o tipo de ação de retenção.
ms.openlocfilehash: cb1cfa8a1306c4a6cacf5c82824d19cab57e7941
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751036"
---
# <a name="actiontype-holdactiontype"></a>ActionType (HoldActionType)

O elemento **ActionType** indica o tipo de ação de retenção. 
  
```XML
<ActionType> Create | Update | Remove </ActionType>
```

 **HoldActionType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[SetHoldOnMailboxes](setholdonmailboxes.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **ActionType** é o tipo de espera definido em uma caixa de correio. Um valor de texto de **criação** indica que uma isenção de caixa de correio será criada. Um valor de texto da **atualização** indica que uma isenção de caixa de correio será atualizada. Um valor de texto de **Remover** indica que uma isenção de caixa de correio será removida. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |false  <br/> |
   

