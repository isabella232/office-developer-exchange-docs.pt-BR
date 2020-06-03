---
title: Estado (TeamMailboxLifecycleStateType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3b1bc531-6988-41c3-9aad-3f5ad5b732a9
description: O elemento State contém o estado do ciclo de vida definido em uma caixa de correio de site.
ms.openlocfilehash: 597946b48649d997f8dd57823b4e0fcc091a6f84
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465160"
---
# <a name="state-teammailboxlifecyclestatetype"></a>Estado (TeamMailboxLifecycleStateType)

O elemento **State** contém o estado do ciclo de vida definido em uma caixa de correio de site. 
  
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

O valor de texto do elemento **State** é o estado do ciclo de vida definido em uma caixa de correio de site. Um valor de texto **ativo** indica que uma caixa de correio de site está em uso ativo. Um valor de texto **fechado** indica que uma caixa de correio de site foi fechada e não está em uso ativo. Um valor de texto **desvinculado** indica que uma caixa de correio de site não está vinculada a um ambiente de colaboração baseado na Web. Os valores **Active**, **Closed**e **PendingDelete** são mutuamente exclusivos, mas o valor **desvinculado** não é mutuamente exclusivo dos outros valores. Um valor de texto de **PendingDelete** indica que uma caixa de correio de site está aguardando a exclusão. Uma caixa de correio de site deve ser fechada para que possa ser definida como **PendingDelete**.
  
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
   

