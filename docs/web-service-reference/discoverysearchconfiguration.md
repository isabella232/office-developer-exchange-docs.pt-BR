---
title: DiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 085384f9-dca4-4534-82e2-dd782471d0da
description: O elemento DiscoverySearchConfiguration especifica a configuração da pesquisa de Descoberta Eletrônica.
ms.openlocfilehash: 4f5f0a5b8e78521302fd136f0a0280aa3ff4e4c3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523094"
---
# <a name="discoverysearchconfiguration"></a>DiscoverySearchConfiguration

O **elemento DiscoverySearchConfiguration** especifica a configuração da pesquisa de Descoberta Eletrônica. 
  
```XML
<DiscoverySearchConfiguration>
    <SearchId></SearchId>
    <SearchQuery></SearchQuery>
    <SearchableMailboxes></SearchableMailboxes>
</DiscoverySearchConfiguration>
```

 **DiscoverySearchConfigurationType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SearchId](searchid.md) <br/> |Especifica o identificador da pesquisa.  <br/> |
|[SearchQuery](searchquery.md) <br/> |Especifica o nome de uma consulta de pesquisa de Descoberta e.  <br/> |
|[SearchableMailboxes](searchablemailboxes.md) <br/> |Contém uma lista das caixas de correio retornadas de uma **solicitação GetSearchableMailboxes.**  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DiscoverySearchConfigurations](discoverysearchconfigurations.md) <br/> |Especifica uma matriz de **elementos DiscoverySearchConfiguration.**  <br/> |
   
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

