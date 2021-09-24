---
title: Position
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 46726ebb-a403-4793-8378-282aa7dc39d0
description: O elemento Position especifica a posição de uma entidade extraída de uma mensagem.
ms.openlocfilehash: 6b4e7c12bbcf12b8804619caa508f5c2c0bc4eda
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515289"
---
# <a name="position"></a>Position

O **elemento Position** especifica a posição de uma entidade extraída de uma mensagem. 
  
```XML
<Position> LatestReply | Other | Subject | Signature </Position>
```

 **EmailPositionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[UrlEntity](urlentity.md)  |  [AddressEntity](addressentity.md)  |  [EmailAddressEntity](emailaddressentity.md)  |  [MeetingSuggestion](meetingsuggestion.md)  |  [Contato (ContactType)](contact-contacttype.md)  |  [Telefone (PhoneEntityType)](phone-phoneentitytype.md)  |  [TaskSuggestion](tasksuggestion.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento Position** é o local onde uma entidade extraída se originou na mensagem de origem. Os valores de texto do elemento **Position** são: 
  
- **LatestReply** - a entidade extraída se origina da resposta mais recente à mensagem. 
    
- **Outro** - a entidade extraída se origina de uma parte indefinida da mensagem. 
    
- **Assunto** - a entidade extraída se origina do assunto da mensagem. 
    
- **Assinatura** - a entidade extraída se origina da assinatura da mensagem. 
    
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
   

