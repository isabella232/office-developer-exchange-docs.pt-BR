---
title: DisableReason
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f41b5be6-9b79-4e83-8cdb-aa779e13cb3f
description: O elemento DisableReason especifica o motivo para desabilitar um aplicativo.
ms.openlocfilehash: 8156dac17e81dd1c3f49575491924185b04d53e9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528833"
---
# <a name="disablereason"></a>DisableReason

O **elemento DisableReason** especifica o motivo para desabilitar um aplicativo. 
  
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
|NoReason  <br/> |Nenhum motivo dado  <br/> |
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
|Nome do esquema  <br/> |Tipo de esquema  <br/> |
|Arquivo de validação  <br/> |types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

