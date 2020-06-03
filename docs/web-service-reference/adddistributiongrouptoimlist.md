---
title: AddDistributionGroupToImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: adbffbfc-e436-4620-acfc-5dfd41a88cb8
description: O elemento AddDistributionGroupToImList define uma solicitação para adicionar uma lista de distribuição a uma lista de mensagens instantâneas.
ms.openlocfilehash: 90a84b23678fb0740158f601967905a8847286fd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460376"
---
# <a name="adddistributiongrouptoimlist"></a>AddDistributionGroupToImList

O elemento **AddDistributionGroupToImList** define uma solicitação para adicionar uma lista de distribuição a uma lista de mensagens instantâneas. 
  
```XML
<AddDistributionGroupToImList>
   <SmtpAddress/>
   <DisplayName/>
</AddDistributionGroupToImList>
```

 **AddDistributionGroupToImListType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[SmtpAddress](smtpaddress.md)  |  [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md)
  
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
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |falso  <br/> |
   

