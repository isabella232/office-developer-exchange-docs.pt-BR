---
title: ExpandGroupMembership
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 8989e96b-8fa1-4858-93b2-2cbdb30b9ca9
description: O elemento ExpandGroupMembership indica se a associação do grupo retornada de uma solicitação GetSearchableMailboxes.
ms.openlocfilehash: fb835f8f1fa9fb957c6b3bf3ddef80e68d9c049f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541396"
---
# <a name="expandgroupmembership"></a>ExpandGroupMembership

O **elemento ExpandGroupMembership** indica se a associação do grupo retornada de uma **solicitação GetSearchableMailboxes.** 
  
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

Um valor de texto **true para** o **elemento ExpandGroupElement** indica que a associação ao grupo é expandida. Um valor **false** indica que a associação ao grupo não é expandida para mostrar os membros do grupo. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode estar vazio  <br/> |falso  <br/> |
   

