---
title: InPlaceHoldConfigurationOnly
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 921ecc73-b7e2-40a7-8458-68f18dd5a13b
description: O elemento InPlaceHoldConfigurationOnly especifica se deve incluir a configuração de espera local.
ms.openlocfilehash: 3b1f12bb2d021693b20c3a9013c889b1a8074e62
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59532921"
---
# <a name="inplaceholdconfigurationonly"></a>InPlaceHoldConfigurationOnly

O **elemento InPlaceHoldConfigurationOnly** especifica se deve incluir a configuração de espera local. 
  
```XML
<InPlaceHoldConfigurationOnly>true | false</InPlaceHoldConfigurationOnly>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md)
  
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** para o **elemento InPlaceHoldConfigurationOnly** indica que a configuração de espera no local está incluída. Um valor **false** indica que a configuração de espera no local não está incluída. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

