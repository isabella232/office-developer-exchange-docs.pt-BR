---
title: SetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fd5b9f0e-23e8-428c-8168-2d6b4ecd6beb
description: O elemento SetHoldOnMailboxes contém uma solicitação SetHoldOnMailboxes.
ms.openlocfilehash: 82ebbbdce04a5b70eae790a899ca089e38aa76d9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516368"
---
# <a name="setholdonmailboxes"></a>SetHoldOnMailboxes

O **elemento SetHoldOnMailboxes** contém uma **solicitação SetHoldOnMailboxes.** 
  
```XML
<SetHoldOnMailboxes>
   <ActionType/>
   <HoldId/>
   <Query/>
   <Mailboxes/>
   <Language/>
   <IncludeNonIndexableItems/>
   <Deduplication/>
   <InPlaceHoldIdentity/>
</SetHoldOnMailboxes>
```

 **SetHoldOnMailboxesType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[ActionType (HoldActionType)](actiontype-holdactiontype.md)  |  [HoldId](holdid.md)  |  [Consulta](query.md)  |  [Caixas de correio (ArrayOfStringsType)](mailboxes-arrayofstringstype.md)  |  [Idioma](language.md)  |  [IncludeNonIndexableItems](includenonindexableitems.md)  |  [Deduplication](deduplication.md)  |  [InPlaceHoldIdentity](inplaceholdidentity.md)
  
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
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
   

