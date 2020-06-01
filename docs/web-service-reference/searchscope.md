---
title: SearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4a53989e-eca6-45c4-afac-4d6ac19597d2
description: O elemento SearchScope especifica o escopo de uma pesquisa.
ms.openlocfilehash: df11c8db418ac90d1166030aeed3672c0b810052
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466861"
---
# <a name="searchscope"></a>SearchScope

O elemento **SearchScope** especifica o escopo de uma pesquisa. 
  
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

O valor de texto do elemento **SearchScope** indica o tipo de caixa de correio pesquisada para uma pesquisa de descoberta. Um valor de texto de **PrimaryOnly** indica que a caixa de correio principal é pesquisada. Um valor de texto de **ArchiveOnly** indica que a caixa de correio de arquivo morto é pesquisada. Um valor de texto indica que as **caixas de correio** primárias e de arquivo morto são pesquisadas. 
  
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
   

