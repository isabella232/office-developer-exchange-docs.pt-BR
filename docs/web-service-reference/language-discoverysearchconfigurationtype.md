---
title: Language (DiscoverySearchConfigurationType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 34eab81c-d832-4925-9f76-d69f24b36931
description: O elemento Language (DiscoverySearchConfigurationType) identifica a cultura a ser usada para o formato específico de cultura de intervalos de datas. Também especifica o idioma usado em uma consulta de pesquisa.
ms.openlocfilehash: 3cf85525147bec5d6dfc6fe2b2af5916d42c44be
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463283"
---
# <a name="language-discoverysearchconfigurationtype"></a>Language (DiscoverySearchConfigurationType)

O elemento **Language (DiscoverySearchConfigurationType)** identifica a cultura a ser usada para o formato específico de cultura de intervalos de datas. Também especifica o idioma usado em uma consulta de pesquisa. 
  
```XML
<Language />
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[DiscoverySearchConfiguration](discoverysearchconfiguration.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **Language (DiscoverySearchConfigurationType)** é uma cultura ou idioma. 
  
## <a name="remarks"></a>Comentários

Este elemento Especifica o formato dos intervalos de datas especificados na [operação SearchMailboxes](searchmailboxes-operation.md) ou na [operação SetHoldOnMailboxes](setholdonmailboxes-operation.md).
  
Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Também consulte



[DiscoverySearchConfiguration](discoverysearchconfiguration.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

