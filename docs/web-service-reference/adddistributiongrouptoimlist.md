---
title: AddDistributionGroupToImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: adbffbfc-e436-4620-acfc-5dfd41a88cb8
description: O elemento AddDistributionGroupToImList define uma solicitação para adicionar uma lista de distribuição a uma lista de mensagens instantâneas.
ms.openlocfilehash: 8b2425a05d184b203f8b65f74a6119d5b6d09946
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525405"
---
# <a name="adddistributiongrouptoimlist"></a>AddDistributionGroupToImList

O **elemento AddDistributionGroupToImList** define uma solicitação para adicionar uma lista de distribuição a uma lista de mensagens instantâneas. 
  
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

Nenhum.
  
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
   

