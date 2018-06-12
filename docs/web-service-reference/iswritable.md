---
title: IsWritable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d4af8eee-7001-4a8e-b9bd-d14882f2406b
description: O elemento IsWritable Especifica se o contato subjacente ou o destinatário do Active Directory pode ser gravado em.
ms.openlocfilehash: 03f258d01ecfc12dfa4e09ac88f4a75340d2acf3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824158"
---
# <a name="iswritable"></a>IsWritable

O elemento **IsWritable** Especifica se o contato subjacente ou o destinatário do Active Directory pode ser gravado em. 
  
```XML
<IsWritable> true | false </IsWritable>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Atribuição (PersonaAttributionType)](attribution-personaattributiontype.md)
  
## <a name="text-value"></a>Text value

Um valor de **true** para o elemento **IsWritable** text indica que o contato ou um objeto do Active Directory está disponível para acesso de gravação. Um valor **false** indica que o contato ou um objeto do Active Directory não está disponível para acesso de gravação. 
  
## <a name="remarks"></a>Coment�rios

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  

