---
title: NonIndexableItemDetailsResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7cbdbc21-5405-4cbc-8ca0-d7b0257927aa
description: O elemento NonIndexableItemDetailsResult especifica os resultados da operação WSDL GetNonIndexableItemDetails.
ms.openlocfilehash: 647f58b5e7285af70bbfb3a203ba71c9a3ccebcc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465440"
---
# <a name="nonindexableitemdetailsresult"></a><span data-ttu-id="05ad7-103">NonIndexableItemDetailsResult</span><span class="sxs-lookup"><span data-stu-id="05ad7-103">NonIndexableItemDetailsResult</span></span>

<span data-ttu-id="05ad7-104">O elemento **NonIndexableItemDetailsResult** especifica os resultados da operação WSDL **GetNonIndexableItemDetails** .</span><span class="sxs-lookup"><span data-stu-id="05ad7-104">The **NonIndexableItemDetailsResult** element specifies the results of the **GetNonIndexableItemDetails** WSDL operation.</span></span> 
  
```XML
<NonIndexableItemDetailsResult>
   <Items/>
   <FailedMailboxes/>
</NonIndexableItemDetailsResult>
```

 <span data-ttu-id="05ad7-105">**NonIndexableItemDetailResultType**</span><span class="sxs-lookup"><span data-stu-id="05ad7-105">**NonIndexableItemDetailResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05ad7-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="05ad7-106">Attributes and elements</span></span>

<span data-ttu-id="05ad7-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="05ad7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05ad7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="05ad7-108">Attributes</span></span>

<span data-ttu-id="05ad7-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="05ad7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05ad7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="05ad7-110">Child elements</span></span>

<span data-ttu-id="05ad7-111">[Itens (ArrayOfNonIndexableItemDetailsType)](items-arrayofnonindexableitemdetailstype.md) , [FailedMailboxes](failedmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="05ad7-111">[Items (ArrayOfNonIndexableItemDetailsType)](items-arrayofnonindexableitemdetailstype.md) , [FailedMailboxes](failedmailboxes.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="05ad7-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="05ad7-112">Parent elements</span></span>

<span data-ttu-id="05ad7-113">[GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md) , [GetNonIndexableItemDetailsResponseMessage](getnonindexableitemdetailsresponsemessage.md)</span><span class="sxs-lookup"><span data-stu-id="05ad7-113">[GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md) , [GetNonIndexableItemDetailsResponseMessage](getnonindexableitemdetailsresponsemessage.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="05ad7-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="05ad7-114">Remarks</span></span>

<span data-ttu-id="05ad7-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="05ad7-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="05ad7-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="05ad7-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05ad7-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="05ad7-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05ad7-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="05ad7-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="05ad7-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="05ad7-119">Schema name</span></span>  <br/> |<span data-ttu-id="05ad7-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="05ad7-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="05ad7-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="05ad7-121">Validation file</span></span>  <br/> |<span data-ttu-id="05ad7-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="05ad7-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="05ad7-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="05ad7-123">Can be empty</span></span>  <br/> |<span data-ttu-id="05ad7-124">False</span><span class="sxs-lookup"><span data-stu-id="05ad7-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05ad7-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="05ad7-125">See also</span></span>



[<span data-ttu-id="05ad7-126">Operação GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="05ad7-126">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)


- [<span data-ttu-id="05ad7-127">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="05ad7-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

