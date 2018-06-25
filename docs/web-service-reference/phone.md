---
title: Telefone
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9381d8e0-b705-49fd-a822-00fb485bdbab
description: O elemento do telefone Especifica um número de telefone único resultante de uma extração de entidade de contato.
ms.openlocfilehash: b10a3af65784dafc4445dfcac33fb4b6372c02ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824747"
---
# <a name="phone"></a>Telefone

O elemento do **telefone** Especifica um número de telefone único resultante de uma extração de entidade de contato. 
  
```XML
<Phone>
   <OriginalPhoneString/>
   <PhoneString/>
   <Type/>
</Phone>
```

 **PhoneType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

[OriginalPhoneString](originalphonestring.md) | [PhoneString](phonestring.md) | [tipo (string)](type-string.md)
  
### <a name="parent-elements"></a>Elementos pai

[PhoneNumbers (ArrayOfPhonesType)](phonenumbers-arrayofphonestype.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

