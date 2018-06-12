---
title: DisableReason
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f41b5be6-9b79-4e83-8cdb-aa779e13cb3f
description: O elemento DisableReason Especifica a razão para desabilitar um aplicativo.
ms.openlocfilehash: f900bd1b98b294900f767c778b9c5f87f74042ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751837"
---
# <a name="disablereason"></a>DisableReason

O elemento **DisableReason** Especifica a razão para desabilitar um aplicativo. 
  
```XML
<DisableReason> NoReason | OutlookClientPerformance | OWAClientPerformance | MobileClientPerformance </DisableReason>
```

 **DisableReasonType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DisableApp](disableapp.md) <br/> |Especifica uma solicitação para desabilitar um aplicativo.  <br/> |
   
## <a name="text-value"></a>Text value

**Valor de texto do elemento DisableReason**

|**Valor**|**Descrição**|
|:-----|:-----|
|NoReason  <br/> |Não há motivo dado  <br/> |
|OutlookClientPerformance  <br/> |Para melhorar o desempenho do cliente de email.  <br/> |
|OWAClientPerformance  <br/> |Para melhorar o desempenho de cliente de aplicativo Web.  <br/> |
|MobileClientPerformance  <br/> |Para melhorar o desempenho do cliente móvel.  <br/> |
   
## <a name="remarks"></a>Coment�rios

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

