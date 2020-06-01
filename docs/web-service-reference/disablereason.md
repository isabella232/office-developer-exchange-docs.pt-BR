---
title: DisableReason
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f41b5be6-9b79-4e83-8cdb-aa779e13cb3f
description: O elemento DisableReason especifica a razão para desabilitar um aplicativo.
ms.openlocfilehash: 1406d69647bde5389dc9bb61adf7537a57d5adfc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463668"
---
# <a name="disablereason"></a>DisableReason

O elemento **DisableReason** especifica a razão para desabilitar um aplicativo. 
  
```XML
<DisableReason> NoReason | OutlookClientPerformance | OWAClientPerformance | MobileClientPerformance </DisableReason>
```

 **DisableReasonType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DisableApp](disableapp.md) <br/> |Especifica uma solicitação para desabilitar um aplicativo.  <br/> |
   
## <a name="text-value"></a>Valor de texto

**Valor de texto do elemento DisableReason**

|**Valor**|**Descrição**|
|:-----|:-----|
|Noreason  <br/> |Nenhum motivo fornecido  <br/> |
|OutlookClientPerformance  <br/> |Para melhorar o desempenho do cliente de email.  <br/> |
|OWAClientPerformance  <br/> |Para melhorar o desempenho do cliente do aplicativo Web.  <br/> |
|MobileClientPerformance  <br/> |Para melhorar o desempenho do cliente móvel.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Também consulte

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

