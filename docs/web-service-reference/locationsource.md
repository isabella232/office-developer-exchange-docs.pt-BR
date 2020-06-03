---
title: Localização
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: O elemento LocalName especifica informações sobre a origem do endereço postal associado, por exemplo, um contato ou um catálogo telefônico.
ms.openlocfilehash: ceba52c43d1c798bb8f5492b779c7c45d7d00b0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467099"
---
# <a name="locationsource"></a>Localização

O elemento **LocalName** especifica informações sobre a origem do endereço postal associado, por exemplo, um contato ou um catálogo telefônico. 
  
```XML
<LocationSource> None | LocationServices | PhonebookServices | Device | Contact | Resource </LocationSource>
```

 **LocationSourceType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Valor (PersonaPostalAddressType)](value-personapostaladdresstype.md)  |  [Address (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)
  
## <a name="text-value"></a>Valor de texto

Os valores de texto para o elemento **LocationName** estão listados na tabela a seguir: 
  
**Valores de texto do elemento local**

|**Valor**|**Descrição**|
|:-----|:-----|
|Nenhum  <br/> |Não há nenhuma origem de local.  <br/> |
|LocalServices  <br/> |As informações foram obtidas dos serviços de localização.  <br/> |
|Catálogos telefônicos  <br/> |As informações foram obtidas de serviços de catálogo telefônico.  <br/> |
|Dispositivo  <br/> |As informações foram obtidas do dispositivo.  <br/> |
|Contato  <br/> |As informações foram obtidas de um contato.  <br/> |
|Resource  <br/> |As informações foram obtidas de um recurso.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  

