---
title: SetImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3c107b8d-714b-4cd5-ad1b-97b7cbcb90d6
description: O elemento SetImGroup representa uma solicitação para alterar o nome de exibição de um grupo de mensagens instantâneo.
ms.openlocfilehash: 67fd8188e3436d5042a2867fe54e673348cba807
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825422"
---
# <a name="setimgroup"></a>SetImGroup

O elemento **SetImGroup** representa uma solicitação para alterar o nome de exibição de um grupo de mensagens instantâneo. 
  
```XML
<SetImGroup>
   <GroupId/>
   <NewDisplayName/>
</SetImGroup>
```

 **SetImGroupType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

[GroupId](groupid.md) | [NewDisplayName](newdisplayname.md)
  
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
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

