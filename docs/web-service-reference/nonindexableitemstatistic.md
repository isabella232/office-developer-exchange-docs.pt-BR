---
title: NonIndexableItemStatistic
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 593e0c79-9ec2-4040-a6a3-3c5c61cbdf7c
description: O elemento NonIndexableItemStatistic contém uma única estatística para um item que não pôde ser indexado
ms.openlocfilehash: 93bdaad2f10adf52ef99f51106596f155af2f18c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509543"
---
# <a name="nonindexableitemstatistic"></a>NonIndexableItemStatistic

O **elemento NonIndexableItemStatistic** contém uma única estatística para um item que não pôde ser indexado 
  
```XML
<NonIndexableItemStatistic>
   <Mailbox/>
   <ItemCount/>
   <ErrorMessage/>
</NonIndexableItemStatistic>
```

 **NonIndexableItemStatisticType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[Caixa de correio (cadeia de caracteres)](mailbox-string.md)  |  [ItemCount](itemcount.md)  |  [ErrorMessage](errormessage.md)
  
### <a name="parent-elements"></a>Elementos pai

[NonIndexableItemStatistics](nonindexableitemstatistics.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   

