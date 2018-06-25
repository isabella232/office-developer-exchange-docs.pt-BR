---
title: InPlaceHoldIdentity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54f45774-00a0-4392-af1b-8c5f2208a53f
description: O elemento InPlaceHoldIdentity Especifica a identidade de uma isenção que preserva os itens de caixa de correio.
ms.openlocfilehash: 954e6ad6c3e0b7786d6bbb8230dba913a32359bc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823938"
---
# <a name="inplaceholdidentity"></a>InPlaceHoldIdentity

O elemento **InPlaceHoldIdentity** Especifica a identidade de uma isenção que preserva os itens de caixa de correio. 
  
```XML
<InPlaceHoldIdentity></InPlaceHoldIdentity>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[SetHoldOnMailboxes](setholdonmailboxes.md) | [DiscoverySearchConfiguration](discoverysearchconfiguration.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **InPlaceHoldIdentity** é o identificador de espera de caixa de correio. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação SetHoldOnMailboxes](setholdonmailboxes-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

