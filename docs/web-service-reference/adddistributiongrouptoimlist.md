---
title: AddDistributionGroupToImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: adbffbfc-e436-4620-acfc-5dfd41a88cb8
description: O elemento de AddDistributionGroupToImList define uma solicitação para adicionar uma lista de distribuição a uma lista de mensagem instantânea.
ms.openlocfilehash: b63daeb8b1d60123215bfcdec307f2f948d2ec39
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751048"
---
# <a name="adddistributiongrouptoimlist"></a>AddDistributionGroupToImList

O elemento de **AddDistributionGroupToImList** define uma solicitação para adicionar uma lista de distribuição a uma lista de mensagem instantânea. 
  
```XML
<AddDistributionGroupToImList>
   <SmtpAddress/>
   <DisplayName/>
</AddDistributionGroupToImList>
```

 **AddDistributionGroupToImListType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

[SmtpAddress](smtpaddress.md) | [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md)
  
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
|Pode estar vazio  <br/> |false  <br/> |
   

