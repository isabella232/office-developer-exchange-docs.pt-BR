---
title: NonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 12f2934a-008c-4236-b8b3-7c7b6b5707e2
description: O elemento NonIndexableItemStatistics contém uma matriz de estatísticas para itens que não puderam ser indexados.
ms.openlocfilehash: 5a11bd4d7ef0c574f26580613063a885530176f9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466728"
---
# <a name="nonindexableitemstatistics"></a><span data-ttu-id="56980-103">NonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="56980-103">NonIndexableItemStatistics</span></span>

<span data-ttu-id="56980-104">O elemento **NonIndexableItemStatistics** contém uma matriz de estatísticas para itens que não puderam ser indexados.</span><span class="sxs-lookup"><span data-stu-id="56980-104">The **NonIndexableItemStatistics** element contains an array of statistics for items that could not be indexed.</span></span> 
  
```XML
<NonIndexableItemStatistics>
   <NonIndexableItemStatistic/>
</NonIndexableItemStatistics>
```

 <span data-ttu-id="56980-105">**ArrayOfNonIndexableItemStatisticsType**</span><span class="sxs-lookup"><span data-stu-id="56980-105">**ArrayOfNonIndexableItemStatisticsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="56980-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="56980-106">Attributes and elements</span></span>

<span data-ttu-id="56980-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="56980-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56980-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="56980-108">Attributes</span></span>

<span data-ttu-id="56980-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="56980-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="56980-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="56980-110">Child elements</span></span>

[<span data-ttu-id="56980-111">NonIndexableItemStatistic</span><span class="sxs-lookup"><span data-stu-id="56980-111">NonIndexableItemStatistic</span></span>](nonindexableitemstatistic.md)
  
### <a name="parent-elements"></a><span data-ttu-id="56980-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="56980-112">Parent elements</span></span>

<span data-ttu-id="56980-113">[GetNonIndexableItemStatisticsResponse](getnonindexableitemstatisticsresponse.md) , [GetNonIndexableItemStatisticsResponseMessage](getnonindexableitemstatisticsresponsemessage.md)</span><span class="sxs-lookup"><span data-stu-id="56980-113">[GetNonIndexableItemStatisticsResponse](getnonindexableitemstatisticsresponse.md) , [GetNonIndexableItemStatisticsResponseMessage](getnonindexableitemstatisticsresponsemessage.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="56980-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="56980-114">Remarks</span></span>

<span data-ttu-id="56980-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="56980-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="56980-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="56980-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="56980-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="56980-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="56980-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="56980-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="56980-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="56980-119">Schema name</span></span>  <br/> |<span data-ttu-id="56980-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="56980-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="56980-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="56980-121">Validation file</span></span>  <br/> |<span data-ttu-id="56980-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="56980-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="56980-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="56980-123">Can be empty</span></span>  <br/> |<span data-ttu-id="56980-124">False</span><span class="sxs-lookup"><span data-stu-id="56980-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="56980-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="56980-125">See also</span></span>



[<span data-ttu-id="56980-126">Operação GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="56980-126">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)


- [<span data-ttu-id="56980-127">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="56980-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

