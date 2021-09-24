---
title: IncludeNonIndexableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: af7f202b-2889-447e-bdeb-aaad18ce6b46
description: O elemento IncludeNonIndexableItems contém um valor Boolean para indicar se deve incluir itens que não podem ser indexados.
ms.openlocfilehash: 33ff8c59c3ef1d9a91f87870e0a876c5a39ce795
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514596"
---
# <a name="includenonindexableitems"></a>IncludeNonIndexableItems

O **elemento IncludeNonIndexableItems** contém um valor **Boolean** para indicar se deve incluir itens que não podem ser indexados. 
  
```XML
<IncludeNonIndexableItems>true | false</IncludeNonIndexableItems>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[SetHoldOnMailboxes](setholdonmailboxes.md)
  
## <a name="text-value"></a>Valor de texto

Um valor de texto **true para** o **elemento IncludeNonIndexableItems** indica que itens que não podem ser indexados estão incluídos com reter caixas de correio. Um valor false indica **que** os itens que não podem ser indexados não estão incluídos em resvasões de caixa de correio. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |falso  <br/> |
   

