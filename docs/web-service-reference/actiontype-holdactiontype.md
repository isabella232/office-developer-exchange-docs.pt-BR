---
title: ActionType (HoldActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f50449b9-e73b-43c5-af96-6433bf434dce
description: O elemento ActionType indica o tipo de ação para a isenção.
ms.openlocfilehash: 8f2796df818dac2bd285b055aa44fbcecd0de5e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457855"
---
# <a name="actiontype-holdactiontype"></a>ActionType (HoldActionType)

O elemento **ActionType** indica o tipo de ação para a isenção. 
  
```XML
<ActionType> Create | Update | Remove </ActionType>
```

 **HoldActionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[SetHoldOnMailboxes](setholdonmailboxes.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **ActionType** é o tipo de retenção definido em uma caixa de correio. Um valor de texto de **Create** indica que uma retenção de caixa de correio será criada. Um valor de texto de **Update** indica que um bloqueio de caixa de correio será atualizado. Um valor de texto **Remove** indica que uma retenção de caixa de correio será removida. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |falso  <br/> |
   

