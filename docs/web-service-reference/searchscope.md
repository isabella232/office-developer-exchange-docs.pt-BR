---
title: SearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 4a53989e-eca6-45c4-afac-4d6ac19597d2
description: O elemento SearchScope especifica o escopo de uma pesquisa.
ms.openlocfilehash: d4caa87cd552a633812b99d7e97f2419b156fb78
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523394"
---
# <a name="searchscope"></a>SearchScope

O **elemento SearchScope** especifica o escopo de uma pesquisa. 
  
```XML
<SearchScope> PrimaryOnly | ArchiveOnly | All </SearchScope>
```

 **MailboxSearchLocationType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[MailboxSearchScope](mailboxsearchscope.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento SearchScope** indica o tipo de caixa de correio que é pesquisado para uma pesquisa de descoberta. Um valor de texto **primaryOnly** indica que a caixa de correio principal é pesquisada. Um valor de texto **de ArchiveOnly** indica que a caixa de correio de arquivo morto é pesquisada. Um valor de texto **de All** indica que as caixas de correio primárias e de arquivo morto são pesquisadas. 
  
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
   

