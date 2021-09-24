---
title: State (TeamMailboxLifecycleStateType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3b1bc531-6988-41c3-9aad-3f5ad5b732a9
description: O elemento State contém o estado do ciclo de vida definido em uma caixa de correio de site.
ms.openlocfilehash: 5189ee8573fd33d2265fd60c47bb40d17b16b8fe
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538965"
---
# <a name="state-teammailboxlifecyclestatetype"></a>State (TeamMailboxLifecycleStateType)

O **elemento State** contém o estado do ciclo de vida definido em uma caixa de correio de site. 
  
```XML
<State> Active | Closed | Unlinked | PendingDelete </State>
```

**TeamMailboxLifecycleStateType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[SetTeamMailbox](setteammailbox.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **State** é o estado do ciclo de vida definido em uma caixa de correio de site. Um valor de texto **do Active** indica que uma caixa de correio de site está em uso ativo. Um valor de texto **de Closed** indica que uma caixa de correio de site foi fechada e não está em uso ativo. Um valor de texto **de Desvinculado** indica que uma caixa de correio de site não está vinculada a um ambiente de colaboração baseado na Web. Os **valores Active**, **Closed** e **PendingDelete** são mutuamente exclusivos, mas o valor **Desvinculado** não é mutuamente exclusivo dos outros valores. Um valor de texto **de PendingDelete** indica que uma caixa de correio de site está aguardando exclusão. Uma caixa de correio de site deve ser fechada antes de poder ser definida como **PendingDelete**.
  
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
   

