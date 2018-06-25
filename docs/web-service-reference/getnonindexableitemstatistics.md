---
title: GetNonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dd16d1fb-d82d-42e5-b64a-bc6c19c48fa8
description: O elemento GetNonIndexableItemStatistics Especifica uma solicitação para recuperar estatísticas de item nonindexable.
ms.openlocfilehash: 4e6f9a0ba94e9946a3910661810bc2c9e748ba9f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752566"
---
# <a name="getnonindexableitemstatistics"></a><span data-ttu-id="bb7a9-103">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="bb7a9-103">GetNonIndexableItemStatistics</span></span>

<span data-ttu-id="bb7a9-104">O elemento **GetNonIndexableItemStatistics** Especifica uma solicitação para recuperar estatísticas de item nonindexable.</span><span class="sxs-lookup"><span data-stu-id="bb7a9-104">The **GetNonIndexableItemStatistics** element specifies a request to retrieve nonindexable item statistics.</span></span> 
  
```XML
<GetNonIndexableItemStatistics>
    <Mailboxes/>
</GetNonIndexableItemStatistics>
```

 <span data-ttu-id="bb7a9-105">**GetNonIndexableItemStatisticsType**</span><span class="sxs-lookup"><span data-stu-id="bb7a9-105">**GetNonIndexableItemStatisticsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bb7a9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="bb7a9-106">Attributes and elements</span></span>

<span data-ttu-id="bb7a9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bb7a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb7a9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="bb7a9-108">Attributes</span></span>

<span data-ttu-id="bb7a9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bb7a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bb7a9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bb7a9-110">Child elements</span></span>

|<span data-ttu-id="bb7a9-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bb7a9-111">**Element**</span></span>|<span data-ttu-id="bb7a9-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bb7a9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb7a9-113">Caixas de correio (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="bb7a9-113">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |<span data-ttu-id="bb7a9-114">Especifica uma matriz de elementos de **caixa de correio** .</span><span class="sxs-lookup"><span data-stu-id="bb7a9-114">Specifies an array of **Mailbox** elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bb7a9-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bb7a9-115">Parent elements</span></span>

<span data-ttu-id="bb7a9-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bb7a9-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bb7a9-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="bb7a9-117">Remarks</span></span>

<span data-ttu-id="bb7a9-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bb7a9-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bb7a9-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="bb7a9-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bb7a9-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="bb7a9-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb7a9-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="bb7a9-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bb7a9-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="bb7a9-122">Schema Name</span></span>  <br/> |<span data-ttu-id="bb7a9-123">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="bb7a9-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="bb7a9-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="bb7a9-124">Validation File</span></span>  <br/> |<span data-ttu-id="bb7a9-125">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bb7a9-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bb7a9-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="bb7a9-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="bb7a9-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="bb7a9-127">See also</span></span>



- [<span data-ttu-id="bb7a9-128">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="bb7a9-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

