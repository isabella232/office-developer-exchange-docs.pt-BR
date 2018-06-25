---
title: Apresentadores
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: O elemento de apresentadores Especifica os apresentadores de uma reunião online.
ms.openlocfilehash: f62b458759e0d8199c98827602d6c3fe16aebeea
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824875"
---
# <a name="presenters"></a>Apresentadores

O elemento de **apresentadores** Especifica os apresentadores de uma reunião online. 
  
```XML
<Presenters> Disabled | Internal | Everyone </Presenters>
```

 **PresentersType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[OnlineMeetingSettings](onlinemeetingsettings.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento de **apresentadores** é o tipo de usuários que pode ser um apresentador de uma reunião online. Os valores de texto para o elemento de **apresentadores** são descritos na tabela a seguir. 
  
**Valores de texto do elemento de apresentadores**

|**Valor**|**Descrição**|
|:-----|:-----|
|Desabilitado  <br/> |Os apresentadores estão desabilitados.  <br/> |
|Interno  <br/> |Somente os participantes internos podem ser apresentadores.  <br/> |
|Todos  <br/> |Qualquer participante pode ser um apresentador.  <br/> |
   
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
   

