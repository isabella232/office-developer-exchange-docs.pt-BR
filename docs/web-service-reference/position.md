---
title: Posição
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46726ebb-a403-4793-8378-282aa7dc39d0
description: O elemento de posição Especifica a posição de uma entidade extraída de uma mensagem.
ms.openlocfilehash: 4bd8f3088891e918e13d5ef1ec8e3e5217cb3fa1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824853"
---
# <a name="position"></a>Posição

O elemento de **posição** Especifica a posição de uma entidade extraída de uma mensagem. 
  
```XML
<Position> LatestReply | Other | Subject | Signature </Position>
```

 **EmailPositionType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[UrlEntity](urlentity.md) | [AddressEntity](addressentity.md) | [EmailAddressEntity](emailaddressentity.md) | [MeetingSuggestion](meetingsuggestion.md) | [contato (ContactType)](contact-contacttype.md) | [telefone (PhoneEntityType)](phone-phoneentitytype.md)  |  [ TaskSuggestion](tasksuggestion.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **posição** é o local onde uma entidade extraída originou na mensagem de origem. Os valores de texto para o elemento de **posição** são: 
  
- **LatestReply** - a entidade extraída se origina a resposta mais recente à mensagem. 
    
- **Outros** - a entidade extraída originado de uma indefinido parte da mensagem. 
    
- **Assunto** - a entidade extraída originado de assunto da mensagem. 
    
- **Assinatura** - a entidade extraída se origina a assinatura da mensagem. 
    
## <a name="remarks"></a>Coment�rios

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

