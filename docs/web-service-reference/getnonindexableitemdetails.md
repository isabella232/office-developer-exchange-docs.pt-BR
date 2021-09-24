---
title: GetNonIndexableItemDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ce3994c1-3bb4-4571-b026-34a6c5705410
description: O elemento GetNonIndexableItemDetails especifica uma solicitação para recuperar detalhes de item não indexáveis.
ms.openlocfilehash: 896b978b9b222454b9e3f016aa0593521e92e33d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533608"
---
# <a name="getnonindexableitemdetails"></a>GetNonIndexableItemDetails

O **elemento GetNonIndexableItemDetails** especifica uma solicitação para recuperar detalhes de item não indexáveis. 
  
```XML
<GetNonIndexableItemDetails>
    <Mailboxes/>
    <PageSize/>
    <PageItemReference/>
    <PageDirection/>
</GetNonIndexableItemDetails>
```

 **GetNonIndexableItemDetailsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Mailboxes (NonEmptyArrayOfLegacyDNsType)](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |Especifica uma matriz de elementos **de Caixa de** Correio.  <br/> |
|[PageSize](pagesize.md) <br/> |Contém o número de itens a serem retornados em uma única página para um resultado de pesquisa.  <br/> |
|[PageItemReference](pageitemreference.md) <br/> |Especifica a referência para um item de página.  <br/> |
|[PageDirection](pagedirection.md) <br/> |Contém a direção da paginação no resultado da pesquisa.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
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

