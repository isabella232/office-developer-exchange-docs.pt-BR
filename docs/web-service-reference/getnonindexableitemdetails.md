---
title: GetNonIndexableItemDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ce3994c1-3bb4-4571-b026-34a6c5705410
description: O elemento GetNonIndexableItemDetails Especifica uma solicitação para recuperar os detalhes do item nonindexable.
ms.openlocfilehash: 0aeda85973aa78eff240a017db58ffb57fc0de06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752560"
---
# <a name="getnonindexableitemdetails"></a>GetNonIndexableItemDetails

O elemento **GetNonIndexableItemDetails** Especifica uma solicitação para recuperar os detalhes do item nonindexable. 
  
```XML
<GetNonIndexableItemDetails>
    <Mailboxes/>
    <PageSize/>
    <PageItemReference/>
    <PageDirection/>
</GetNonIndexableItemDetails>
```

 **GetNonIndexableItemDetailsType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Caixas de correio (NonEmptyArrayOfLegacyDNsType)](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |Especifica uma matriz de elementos de **caixa de correio** .  <br/> |
|[PageSize](pagesize.md) <br/> |Contém o número de itens a serem retornados em uma única página para um resultado de pesquisa.  <br/> |
|[PageItemReference](pageitemreference.md) <br/> |Especifica a referência para um item de página.  <br/> |
|[PageDirection](pagedirection.md) <br/> |Contém a direção da paginação no resultado da pesquisa.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagem  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

