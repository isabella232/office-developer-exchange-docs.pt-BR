---
title: Idioma (DiscoverySearchConfigurationType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 34eab81c-d832-4925-9f76-d69f24b36931
description: O elemento de idioma (DiscoverySearchConfigurationType) identifica a cultura a ser usado para o formato de específico da cultura dos intervalos de data. Ela também especifica o idioma usado em uma consulta de pesquisa.
ms.openlocfilehash: 1e904ac4d7f525b2d12cfe83f0da33b9ed474066
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824197"
---
# <a name="language-discoverysearchconfigurationtype"></a>Idioma (DiscoverySearchConfigurationType)

O elemento de **idioma (DiscoverySearchConfigurationType)** identifica a cultura a ser usado para o formato de específico da cultura dos intervalos de data. Ela também especifica o idioma usado em uma consulta de pesquisa. 
  
```XML
<Language />
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[DiscoverySearchConfiguration](discoverysearchconfiguration.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento de **idioma (DiscoverySearchConfigurationType)** é um idioma ou cultura. 
  
## <a name="remarks"></a>Comentários

Este elemento Especifica o formato de intervalos de data especificado na [operação SearchMailboxes](searchmailboxes-operation.md) ou a [operação SetHoldOnMailboxes](setholdonmailboxes-operation.md).
  
Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



[DiscoverySearchConfiguration](discoverysearchconfiguration.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

