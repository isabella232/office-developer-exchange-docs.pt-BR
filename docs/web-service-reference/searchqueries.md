---
title: SearchQueries
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 67328dab-321b-45ad-929e-cd83e65ad87e
description: O elemento SearchQueries contém uma lista de caixas de correio e consultas associadas para pesquisa de descoberta.
ms.openlocfilehash: 66015d71238b4a1055a71aff539ca50150f2a247
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466910"
---
# <a name="searchqueries"></a>SearchQueries

O elemento **SearchQueries** contém uma lista de caixas de correio e consultas associadas para pesquisa de descoberta. 
  
```XML
<SearchQueries>
   <MailboxQuery/>
</SearchQueries>
```

 ****
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[MailboxQuery](mailboxquery.md)
  
### <a name="parent-elements"></a>Elementos pai

[SearchMailboxes](searchmailboxes.md)  |  [SearchMailboxesResult](searchmailboxesresult.md)
  
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
   

