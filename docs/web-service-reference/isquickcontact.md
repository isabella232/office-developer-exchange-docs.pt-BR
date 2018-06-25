---
title: IsQuickContact
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1c9542d6-ef72-4743-828a-bb671e783836
description: O elemento IsQuickContact Especifica um valor Boolean que indica se o contato subjacente é um contato rápido.
ms.openlocfilehash: 979dbd3c0358eacd443eed79b258f7dd6bb9bc7d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824092"
---
# <a name="isquickcontact"></a>IsQuickContact

O elemento **IsQuickContact** Especifica um valor Boolean que indica se o contato subjacente é um contato rápido. 
  
```XML
<IsQuickContact>true | false</IsQuickContact>
```

 **boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Atribuição (PersonaAttributionType)](attribution-personaattributiontype.md) <br/> |Especifica uma instância em uma matriz de atributos de um elemento de **pessoa** .  <br/> |
   
## <a name="text-value"></a>Text value

Um valor de texto de **true** para o elemento **IsQuickContact** indica que o contato é um contato rápido. Um valor **false** indica que o contato não é um contato rápido. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |false  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

