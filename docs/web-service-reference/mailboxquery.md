---
title: MailboxQuery
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e4b496f7-63fa-479a-b045-73276573f64f
description: O elemento MailboxQuery Especifica uma consulta e o escopo de uma pesquisa de descoberta.
ms.openlocfilehash: 371cddd8c4f01525b654f0ad9788cf9dd62ac888
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824295"
---
# <a name="mailboxquery"></a>MailboxQuery

O elemento **MailboxQuery** Especifica uma consulta e o escopo de uma pesquisa de descoberta. 
  
```XML
<MailboxQuery>
   <Query/>
   <MailboxSearchScopes/>
</MailboxQuery>
```

**MailboxQueryType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

[Consulta](query.md) | [MailboxSearchScopes](mailboxsearchscopes.md)
  
### <a name="parent-elements"></a>Elementos pai

[SearchQueries](searchqueries.md)
  
## <a name="remarks"></a>Coment�rios

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

