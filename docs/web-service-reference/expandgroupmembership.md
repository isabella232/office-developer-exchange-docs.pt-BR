---
title: ExpandGroupMembership
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8989e96b-8fa1-4858-93b2-2cbdb30b9ca9
description: O elemento ExpandGroupMembership indica se deve expandir a associação do grupo retornado de uma solicitação GetSearchableMailboxes.
ms.openlocfilehash: 8a94aa3da165ecc13282127e75c8d166f3972ead
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456903"
---
# <a name="expandgroupmembership"></a>ExpandGroupMembership

O elemento **ExpandGroupMembership** indica se deve expandir a associação do grupo retornado de uma solicitação **GetSearchableMailboxes** . 
  
```XML
<ExpandGroupMembership>true | false</ExpandGroupMembership>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md)  |  [GetSearchableMailboxes](getsearchablemailboxes.md)
  
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** para o elemento **ExpandGroupElement** indica que a associação de grupo está expandida. Um valor **false** indica que a associação ao grupo não é expandida para mostrar os membros do grupo. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages. xsd  <br/> |
|Pode estar vazio  <br/> |falso  <br/> |
   

