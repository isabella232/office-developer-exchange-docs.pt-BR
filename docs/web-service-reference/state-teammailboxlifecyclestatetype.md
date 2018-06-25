---
title: Estado (TeamMailboxLifecycleStateType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3b1bc531-6988-41c3-9aad-3f5ad5b732a9
description: O elemento de estado contém o estado de ciclo de vida for definido em uma caixa de correio do site.
ms.openlocfilehash: accd70d36cc34e7364387b98a2e94c56b91f012f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825571"
---
# <a name="state-teammailboxlifecyclestatetype"></a>Estado (TeamMailboxLifecycleStateType)

O elemento de **estado** contém o estado de ciclo de vida for definido em uma caixa de correio do site. 
  
```XML
<State> Active | Closed | Unlinked | PendingDelete </State>
```

**TeamMailboxLifecycleStateType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[SetTeamMailbox](setteammailbox.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento de **estado** é o estado de ciclo de vida que é definido em uma caixa de correio do site. Um valor de texto de **ativo** indica que uma caixa de correio de site está em uso ativo. Um valor de texto **fechado** indica que uma caixa de correio de site foi fechada e não está em uso ativo. Um valor de texto de **desvinculados** indica que uma caixa de correio de site não estiver vinculada a um ambiente de colaboração baseado na web. Os valores de **ativo**, **fechado**e **PendingDelete** são mutuamente exclusivos, mas o valor **desvinculados** não é mutuamente exclusivos os outros valores. Um valor de texto de **PendingDelete** indica que uma caixa de correio de site é exclusão pendente. Uma caixa de correio de site deve ser fechado antes que ela pode ser definida como **PendingDelete**.
  
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
   

