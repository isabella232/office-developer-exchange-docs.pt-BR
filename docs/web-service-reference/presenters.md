---
title: Apresentadores
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: O elemento apresentadores especifica os apresentadores de uma reunião online.
ms.openlocfilehash: 0236457020dfc4684569e84d3d54e357af00d102
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529907"
---
# <a name="presenters"></a>Apresentadores

O elemento **apresentadores** especifica os apresentadores de uma reunião online. 
  
```XML
<Presenters> Disabled | Internal | Everyone </Presenters>
```

 **PresentersType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[OnlineMeetingSettings](onlinemeetingsettings.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **apresentadores** é o tipo de usuários que podem ser um apresentador para uma reunião online. Os valores de texto para o elemento **apresentadores** são descritos na tabela a seguir. 
  
**Valores de texto do elemento apresentadores**

|**Valor**|**Descrição**|
|:-----|:-----|
|Desabilitado  <br/> |Os apresentadores estão desabilitados.  <br/> |
|Interno  <br/> |Somente os participantes internos podem ser apresentadores.  <br/> |
|Todos  <br/> |Qualquer participante pode ser um apresentador.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> ||
   

