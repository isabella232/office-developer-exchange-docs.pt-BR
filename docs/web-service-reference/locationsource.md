---
title: LocationSource
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: O elemento LocationSource Especifica as informações sobre a origem do endereço associado postal, por exemplo, um contato ou um catálogo de telefone.
ms.openlocfilehash: 7f5cf5fcca0a72287593349fcf5090a74225d012
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824248"
---
# <a name="locationsource"></a>LocationSource

O elemento **LocationSource** Especifica as informações sobre a origem do endereço associado postal, por exemplo, um contato ou um catálogo de telefone. 
  
```XML
<LocationSource> None | LocationServices | PhonebookServices | Device | Contact | Resource </LocationSource>
```

 **LocationSourceType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Valor (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [Address (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)
  
## <a name="text-value"></a>Text value

Os valores de texto para o elemento **LocationSource** estão listados na tabela a seguir: 
  
**Valores de texto do elemento LocationSource**

|**Valor**|**Descrição**|
|:-----|:-----|
|None  <br/> |Não há fonte local.  <br/> |
|LocationServices  <br/> |As informações foram obtidas dos serviços de local.  <br/> |
|PhonebookServices  <br/> |As informações foram obtidas dos serviços de catálogo telefônico.  <br/> |
|Dispositivo  <br/> |As informações foram obtidas do dispositivo.  <br/> |
|Contato  <br/> |As informações foi obtidas de um contato.  <br/> |
|Recurso  <br/> |As informações foi obtidas de um recurso.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  

