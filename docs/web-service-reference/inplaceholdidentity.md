---
title: InPlaceHoldIdentity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54f45774-00a0-4392-af1b-8c5f2208a53f
description: O elemento InPlaceHoldIdentity especifica a identidade de uma retenção que preserva os itens da caixa de correio.
ms.openlocfilehash: a06f72e478e7dc5bd1a499dceefeb352b14d7362
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466091"
---
# <a name="inplaceholdidentity"></a>InPlaceHoldIdentity

O elemento **InPlaceHoldIdentity** especifica a identidade de uma retenção que preserva os itens da caixa de correio. 
  
```XML
<InPlaceHoldIdentity></InPlaceHoldIdentity>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[SetHoldOnMailboxes](setholdonmailboxes.md)  |  [DiscoverySearchConfiguration](discoverysearchconfiguration.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **InPlaceHoldIdentity** é o identificador de retenção de caixa de correio. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação SetHoldOnMailboxes](setholdonmailboxes-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

