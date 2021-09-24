---
title: Language (DiscoverySearchConfigurationType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 34eab81c-d832-4925-9f76-d69f24b36931
description: O elemento Language (DiscoverySearchConfigurationType) identifica a cultura a ser usada para o formato específico da cultura de intervalos de datas. Ele também especifica o idioma usado em uma consulta de pesquisa.
ms.openlocfilehash: 5d51960aa00b2c47d96972abc05e4d6027eeecb3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540892"
---
# <a name="language-discoverysearchconfigurationtype"></a>Language (DiscoverySearchConfigurationType)

O **elemento Language (DiscoverySearchConfigurationType)** identifica a cultura a ser usada para o formato específico da cultura de intervalos de datas. Ele também especifica o idioma usado em uma consulta de pesquisa. 
  
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

O valor de texto **do elemento Language (DiscoverySearchConfigurationType)** é uma cultura ou idioma. 
  
## <a name="remarks"></a>Comentários

Este elemento especifica o formato dos intervalos de data especificados na operação [SearchMailboxes](searchmailboxes-operation.md) ou na [operação SetHoldOnMailboxes](setholdonmailboxes-operation.md).
  
Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[DiscoverySearchConfiguration](discoverysearchconfiguration.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

