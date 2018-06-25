---
title: GetSearchableMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 949871f7-0d10-498e-84aa-f0652f1193be
description: O elemento GetSearchableMailboxes contém uma solicitação para obter uma lista de caixas de correio que o cliente tem permissão para executar uma pesquisa de descoberta eletrônica.
ms.openlocfilehash: 8cce18bb62d3840cb9883d20a380cc4f2193303e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752616"
---
# <a name="getsearchablemailboxes"></a>GetSearchableMailboxes

O elemento **GetSearchableMailboxes** contém uma solicitação para obter uma lista de caixas de correio que o cliente tem permissão para executar uma pesquisa de descoberta eletrônica. 
  
```XML
<GetSearchableMailboxes>
   <SearchFilter/>
   <ExpandGroupMembership/>
</GetSearchableMailboxes>
```

 **GetSearchableMailboxesType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

[SearchFilter](searchfilter.md) | [ExpandGroupMembership](expandgroupmembership.md)
  
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

