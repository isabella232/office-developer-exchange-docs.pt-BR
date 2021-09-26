---
title: IncludePersonalArchive
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b373bb1a-6b1d-4959-98a1-4c4ea62973bc
description: O elemento IncludePersonalArchive especifica se o arquivo pessoal deve ser incluído na pesquisa.
ms.openlocfilehash: 2567475fbb2542c7d01e651f2d348f6f91d50b78
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547215"
---
# <a name="includepersonalarchive"></a>IncludePersonalArchive

O **elemento IncludePersonalArchive** especifica se o arquivo pessoal deve ser incluído na pesquisa. 
  
```XML
<IncludePersonalArchive>true | false</IncludePersonalArchive>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindMailboxStatisticsByKeywords](findmailboxstatisticsbykeywords.md) <br/> |Especifica uma solicitação para pesquisar estatísticas de caixa de correio por palavra-chave.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** para **o elemento IncludePersonalArchive** indica que o arquivo morto pessoal está incluído na pesquisa. Um valor **false** indica que o arquivo morto pessoal não está incluído na pesquisa. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

