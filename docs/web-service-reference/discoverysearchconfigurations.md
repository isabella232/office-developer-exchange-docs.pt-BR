---
title: DiscoverySearchConfigurations
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f04b14c9-384c-4016-b113-52a49e15e73b
description: O elemento DiscoverySearchConfigurations especifica uma matriz de elementos DiscoverySearchConfiguration.
ms.openlocfilehash: 0bb104451d4bfe24e5e1bc9c5d2c98f226794c22
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535530"
---
# <a name="discoverysearchconfigurations"></a>DiscoverySearchConfigurations

O **elemento DiscoverySearchConfigurations** especifica uma matriz de **elementos DiscoverySearchConfiguration.** 
  
```XML
<DiscoverySearchConfigurations>
    <DiscoverySearchConfiguration></DiscoverySearchConfiguration>
</DiscoverySearchConfigurations>
```

 **ArrayOfDiscoverySearchConfigurationType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DiscoverySearchConfiguration](discoverysearchconfiguration.md) <br/> |Especifica a configuração da pesquisa de Descoberta Eletrônica.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetDiscoverySearchConfigurationResponseMessage](getdiscoverysearchconfigurationresponsemessage.md) <br/> |Especifica a mensagem de resposta para uma **solicitação GetDiscoverySearchConfiguration.**  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

