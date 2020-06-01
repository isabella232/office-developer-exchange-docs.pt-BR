---
title: GetNonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dd16d1fb-d82d-42e5-b64a-bc6c19c48fa8
description: O elemento GetNonIndexableItemStatistics especifica uma solicitação para recuperar estatísticas de itens não indexados.
ms.openlocfilehash: 4b605379f20f5558566f1cfbad9ef1aa33b6fce6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452787"
---
# <a name="getnonindexableitemstatistics"></a><span data-ttu-id="61aea-103">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="61aea-103">GetNonIndexableItemStatistics</span></span>

<span data-ttu-id="61aea-104">O elemento **GetNonIndexableItemStatistics** especifica uma solicitação para recuperar estatísticas de itens não indexados.</span><span class="sxs-lookup"><span data-stu-id="61aea-104">The **GetNonIndexableItemStatistics** element specifies a request to retrieve nonindexable item statistics.</span></span> 
  
```XML
<GetNonIndexableItemStatistics>
    <Mailboxes/>
</GetNonIndexableItemStatistics>
```

 <span data-ttu-id="61aea-105">**GetNonIndexableItemStatisticsType**</span><span class="sxs-lookup"><span data-stu-id="61aea-105">**GetNonIndexableItemStatisticsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="61aea-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="61aea-106">Attributes and elements</span></span>

<span data-ttu-id="61aea-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="61aea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="61aea-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="61aea-108">Attributes</span></span>

<span data-ttu-id="61aea-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61aea-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="61aea-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="61aea-110">Child elements</span></span>

|<span data-ttu-id="61aea-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="61aea-111">**Element**</span></span>|<span data-ttu-id="61aea-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="61aea-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61aea-113">Caixas de correio (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="61aea-113">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |<span data-ttu-id="61aea-114">Especifica uma matriz de elementos de **caixa de correio** .</span><span class="sxs-lookup"><span data-stu-id="61aea-114">Specifies an array of **Mailbox** elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="61aea-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="61aea-115">Parent elements</span></span>

<span data-ttu-id="61aea-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61aea-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="61aea-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="61aea-117">Remarks</span></span>

<span data-ttu-id="61aea-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="61aea-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="61aea-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="61aea-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="61aea-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="61aea-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="61aea-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="61aea-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="61aea-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="61aea-122">Schema Name</span></span>  <br/> |<span data-ttu-id="61aea-123">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="61aea-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="61aea-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="61aea-124">Validation File</span></span>  <br/> |<span data-ttu-id="61aea-125">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="61aea-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="61aea-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="61aea-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="61aea-127">Também consulte</span><span class="sxs-lookup"><span data-stu-id="61aea-127">See also</span></span>



- [<span data-ttu-id="61aea-128">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="61aea-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

