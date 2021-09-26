---
title: LocationSource
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: O elemento LocationSource especifica informações sobre a origem do endereço postal associado, por exemplo, um contato ou um livro telefônico.
ms.openlocfilehash: f3569494d3e662fbc46060944c8bd399b62d656b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543258"
---
# <a name="locationsource"></a>LocationSource

O **elemento LocationSource** especifica informações sobre a origem do endereço postal associado, por exemplo, um contato ou um livro telefônico. 
  
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

[Valor (PersonaPostalAddressType)](value-personapostaladdresstype.md)  |  [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)
  
## <a name="text-value"></a>Valor de texto

Os valores de texto do **elemento LocationSource** estão listados na tabela a seguir: 
  
**Valores de texto do elemento LocationSource**

|**Valor**|**Descrição**|
|:-----|:-----|
|Nenhum  <br/> |Não há fonte de localização.  <br/> |
|LocationServices  <br/> |As informações foram obtidas dos serviços de localização.  <br/> |
|PhonebookServices  <br/> |As informações foram obtidas dos serviços de lista telefônica.  <br/> |
|Dispositivo  <br/> |As informações foram obtidas do dispositivo.  <br/> |
|Contact  <br/> |As informações foram obtidas de um contato.  <br/> |
|Recurso  <br/> |As informações foram obtidas de um recurso.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  

