---
title: UnifiedMessagingConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnifiedMessagingConfiguration
api_type:
- schema
ms.assetid: cbdb4268-077e-44ed-8ec2-9d759c84cc6d
description: O elemento UnifiedMessagingConfiguration contém informações de configuração de serviço para o serviço de Unificação de mensagens.
ms.openlocfilehash: 3f9f4ed65721929c552615c07e2239f48ef837f3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528689"
---
# <a name="unifiedmessagingconfiguration"></a>UnifiedMessagingConfiguration

O elemento **UnifiedMessagingConfiguration** contém informações de configuração de serviço para o serviço de Unificação de mensagens. 
  
```XML
<UnifiedMessagingConfiguration>
   <UmEnabled/>
   <PlayOnPhoneDialString/>
   <PlayOnPhoneEnabled/>
</UnifiedMessagingConfiguration>
```

 **UnifiedMessageServiceConfiguration**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UmEnabled](umenabled.md) <br/> |Indica se a Unificação de mensagens está habilitada para uma conta. Este elemento é obrigatório.  <br/> |
|[PlayOnPhoneDialString (serviços Web do Exchange)](playonphonedialstring-exchange-web-services.md) <br/> |Identifica a cadeia de caracteres de discagem de reprodução no telefone. Este elemento é obrigatório.  <br/> |
|[PlayOnPhoneEnabled](playonphoneenabled.md) <br/> |Indica se o recurso de reproduzir no telefone está habilitado. Este elemento é obrigatório.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Contém definições de configuração de serviço.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

