---
title: MailboxSearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ef4a4203-61e5-46b8-9fa4-d1a10e785aa2
description: O elemento MailboxSearchScope especifica uma caixa de correio e um escopo de pesquisa para uma pesquisa de descoberta.
ms.openlocfilehash: 832992e4e1dcf96029be4228906b2762f11f3fbe
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544119"
---
# <a name="mailboxsearchscope"></a>MailboxSearchScope

O **elemento MailboxSearchScope** especifica uma caixa de correio e um escopo de pesquisa para uma pesquisa de descoberta. 
  
```XML
<MailboxSearchScope>
   <Mailbox/>
   <SearchScope/>
<MailboxSearchScope>
```

**MailboxSearchScopeType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[Caixa de correio (cadeia de caracteres)](mailbox-string.md)  |  [SearchScope](searchscope.md)
  
### <a name="parent-elements"></a>Elementos pai

[MailboxSearchScopes](mailboxsearchscopes.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

