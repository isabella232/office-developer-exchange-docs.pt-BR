---
title: AddNewImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d5913619-0c13-429d-b9d2-057e8af220f1
description: O elemento AddNewImContactToGroup define uma solicitação para adicionar um novo contato de sistema de mensagens instantâneas a um grupo de mensagens instantâneas.
ms.openlocfilehash: c493ba81b23832a462acd425eb60297801f8768f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463647"
---
# <a name="addnewimcontacttogroup"></a>AddNewImContactToGroup

O elemento **AddNewImContactToGroup** define uma solicitação para adicionar um novo contato de sistema de mensagens instantâneas a um grupo de mensagens instantâneas. 
  
```XML
<AddNewImContactToGroup>
   <ImAddress/>
   <DisplayName/>
   <GroupId/>
</AddNewImContactToGroup>
```

 **AddNewImContactToGroupType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[IMAddress (NonEmptyStringType)](imaddress-nonemptystringtype.md)  |  [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md)  |  [GroupId](groupid.md)
  
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
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
   

