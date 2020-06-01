---
title: Iswritable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d4af8eee-7001-4a8e-b9bd-d14882f2406b
description: O elemento iswritable especifica se o contato subjacente ou o destinatário do Active Directory pode ser gravado.
ms.openlocfilehash: 96075adc1772027456f8829eee43bdc734644c09
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467568"
---
# <a name="iswritable"></a>Iswritable

O elemento **iswritable** especifica se o contato subjacente ou o destinatário do Active Directory pode ser gravado. 
  
```XML
<IsWritable> true | false </IsWritable>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Atribuição (PersonaAttributionType)](attribution-personaattributiontype.md)
  
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** para o elemento **iswritable** indica que o contato ou o objeto do Active Directory está disponível para acesso de gravação. Um valor **false** indica que o contato ou o objeto do Active Directory não está disponível para acesso de gravação. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  

