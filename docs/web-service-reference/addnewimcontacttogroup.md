---
title: AddNewImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: d5913619-0c13-429d-b9d2-057e8af220f1
description: O elemento AddNewImContactToGroup define uma solicitação para adicionar um novo contato de mensagens instantâneas a um grupo de mensagens instantâneas.
ms.openlocfilehash: 48d4fe37964a2851a32398425ed4fbd5d5d4f77d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541564"
---
# <a name="addnewimcontacttogroup"></a>AddNewImContactToGroup

O **elemento AddNewImContactToGroup** define uma solicitação para adicionar um novo contato de mensagens instantâneas a um grupo de mensagens instantâneas. 
  
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

[ImAddress (NonEmptyStringType)](imaddress-nonemptystringtype.md)  |  [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md)  |  [GroupId](groupid.md)
  
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
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode estar vazio  <br/> |falso  <br/> |
   

