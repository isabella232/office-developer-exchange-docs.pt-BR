---
title: Apresentadores
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: O elemento Apresentadores especifica os apresentadores de uma reunião online.
ms.openlocfilehash: 1c9bf9093450e675245b647c98d7b1d00101ce9e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519139"
---
# <a name="presenters"></a>Apresentadores

O **elemento Apresentadores** especifica os apresentadores de uma reunião online. 
  
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

O valor de texto **do elemento Apresentadores** é o tipo de usuários que podem ser apresentadores de uma reunião online. Os valores de texto do elemento **Apresentadores** são descritos na tabela a seguir. 
  
**Valores de texto do elemento Apresentadores**

|**Valor**|**Descrição**|
|:-----|:-----|
|Desabilitada  <br/> |Os apresentadores estão desabilitados.  <br/> |
|Interno  <br/> |Somente participantes internos podem ser apresentadores.  <br/> |
|Todos  <br/> |Qualquer participante pode ser apresentador.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

