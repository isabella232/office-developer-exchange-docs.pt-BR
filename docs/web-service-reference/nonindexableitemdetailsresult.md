---
title: NonIndexableItemDetailsResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 7cbdbc21-5405-4cbc-8ca0-d7b0257927aa
description: O elemento NonIndexableItemDetailsResult especifica os resultados da operação WSDL GetNonIndexableItemDetails.
ms.openlocfilehash: 16f3c8a74f635fdd8204fe207777b4b30bc4d2ed
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539275"
---
# <a name="nonindexableitemdetailsresult"></a>NonIndexableItemDetailsResult

O **elemento NonIndexableItemDetailsResult** especifica os resultados da operação WSDL **GetNonIndexableItemDetails.** 
  
```XML
<NonIndexableItemDetailsResult>
   <Items/>
   <FailedMailboxes/>
</NonIndexableItemDetailsResult>
```

 **NonIndexableItemDetailResultType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[Items (ArrayOfNonIndexableItemDetailsType)](items-arrayofnonindexableitemdetailstype.md) , [FailedMailboxes](failedmailboxes.md)
  
### <a name="parent-elements"></a>Elementos pai

[GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md) , [GetNonIndexableItemDetailsResponseMessage](getnonindexableitemdetailsresponsemessage.md)
  
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
   
## <a name="see-also"></a>Confira também



[Operação GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

