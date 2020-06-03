---
title: Contato
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactSource
api_type:
- schema
ms.assetid: 500b0423-864e-4cde-a39b-6b5b06d1aa6a
description: O elemento ContactName descreve se o contato está localizado no repositório do Exchange ou nos serviços de domínio do Active Directory (AD DS).
ms.openlocfilehash: 5447dedf199c5ad6b944aa33e6dca03e83a3c340
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462707"
---
# <a name="contactsource"></a>Contato

O elemento **ContactName** descreve se o contato está localizado no repositório do Exchange ou nos serviços de domínio do Active Directory (AD DS). 
  
```xml
<ContactSource/>
```

 **ContactSourceType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Contato](contact.md) <br/> |Representa um item de contato no repositório do Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Estes são os valores possíveis para este elemento:
  
- ActiveDirectory
    
- Repositório
    
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

