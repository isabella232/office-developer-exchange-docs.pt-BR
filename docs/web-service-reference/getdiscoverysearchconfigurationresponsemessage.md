---
title: GetDiscoverySearchConfigurationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1b84a4c6-cb0a-4bca-85b2-fec32227930b
description: O elemento GetDiscoverySearchConfigurationResponseMessage especifica a mensagem de resposta para uma solicitação GetDiscoverySearchConfiguration.
ms.openlocfilehash: 23d1c5b7a61a9161d7383ec8b38cd0ebbebfc8cf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460971"
---
# <a name="getdiscoverysearchconfigurationresponsemessage"></a>GetDiscoverySearchConfigurationResponseMessage

O elemento **GetDiscoverySearchConfigurationResponseMessage** especifica a mensagem de resposta para uma solicitação **GetDiscoverySearchConfiguration** . 
  
```XML
<GetDiscoverySearchConfigurationResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DiscoverySearchConfigurations/>
</GetDiscoverySearchConfigurationResponseMessage>
```

 **GetDiscoverySearchConfigurationResponseMessageType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [DescriptiveLinkKey](descriptivelinkkey.md)  |  [MessageXml](messagexml.md)  |  [DiscoverySearchConfigurations](discoverysearchconfigurations.md)
  
### <a name="parent-elements"></a>Elementos pai

[ResponseMessages](responsemessages.md)
  
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
   

