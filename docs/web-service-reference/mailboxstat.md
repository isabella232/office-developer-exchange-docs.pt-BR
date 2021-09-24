---
title: MailboxStat
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5f24dc30-3ac2-4c82-9dfc-be9dbdb585be
description: O elemento MailboxStat especifica estatísticas de uma caixa de correio pesquisada pela pesquisa de descoberta.
ms.openlocfilehash: d48f033df4cfec47313ce690acd19d916b963c00
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522807"
---
# <a name="mailboxstat"></a>MailboxStat

O **elemento MailboxStat** especifica estatísticas de uma caixa de correio pesquisada pela pesquisa de descoberta. 
  
```XML
<MailboxStat>
   <MailboxId/>
   <DisplayName/>
   <ItemCount/>
   <Size/>
</MailboxStat>
```

**MailboxStatisticsItemType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[MailboxId](mailboxid.md)  |  [DisplayName (cadeia de caracteres)](displayname-string.md)  |  [ItemCount](itemcount.md)  |  [Tamanho (longo)](size-long.md)
  
### <a name="parent-elements"></a>Elementos pai

[MailboxStats](mailboxstats.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |falso  <br/> |
   

