---
title: IsWritable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: d4af8eee-7001-4a8e-b9bd-d14882f2406b
description: O elemento IsWritable especifica se o contato subjacente ou o destinatário do Active Directory pode ser gravado.
ms.openlocfilehash: 2663e18f2589516f304930b86a717455b6ab77c3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516710"
---
# <a name="iswritable"></a>IsWritable

O **elemento IsWritable** especifica se o contato subjacente ou o destinatário do Active Directory pode ser gravado. 
  
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

[Attribution (PersonaAttributionType)](attribution-personaattributiontype.md)
  
## <a name="text-value"></a>Valor de texto

Um valor de texto **true para** o **elemento IsWritable** indica que o objeto contact ou Active Directory está disponível para acesso de gravação. Um valor **false** indica que o contato ou o objeto Active Directory não está disponível para acesso a gravação. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  

