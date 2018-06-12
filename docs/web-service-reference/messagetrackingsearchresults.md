---
title: MessageTrackingSearchResults
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingSearchResults
api_type:
- schema
ms.assetid: 6bf36f37-c2b3-40c1-a4df-31573ed8642a
description: O elemento MessageTrackingSearchResults contém uma lista de registros que correspondem aos critérios de pesquisa.
ms.openlocfilehash: 866cc8d4e9afa8347eb7bd0d9e9acaddc616c396
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824454"
---
# <a name="messagetrackingsearchresults"></a><span data-ttu-id="3a5ad-103">MessageTrackingSearchResults</span><span class="sxs-lookup"><span data-stu-id="3a5ad-103">MessageTrackingSearchResults</span></span>

<span data-ttu-id="3a5ad-104">O elemento **MessageTrackingSearchResults** contém uma lista de registros que correspondem aos critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="3a5ad-104">The **MessageTrackingSearchResults** element contains a list of records that match the search criteria.</span></span> 
  
```XML
<MessageTrackingSearchResults>
   <MessageTrackingSearchResult/>
</MessageTrackingSearchResults>
```

 <span data-ttu-id="3a5ad-105">**ArrayOfFindMessageTrackingSearchResultType**</span><span class="sxs-lookup"><span data-stu-id="3a5ad-105">**ArrayOfFindMessageTrackingSearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a5ad-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3a5ad-106">Attributes and elements</span></span>

<span data-ttu-id="3a5ad-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3a5ad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a5ad-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3a5ad-108">Attributes</span></span>

<span data-ttu-id="3a5ad-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3a5ad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a5ad-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3a5ad-110">Child elements</span></span>

|<span data-ttu-id="3a5ad-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3a5ad-111">**Element**</span></span>|<span data-ttu-id="3a5ad-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3a5ad-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a5ad-113">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="3a5ad-113">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="3a5ad-114">Contém um resultado de mensagem única de um elemento [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="3a5ad-114">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3a5ad-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3a5ad-115">Parent elements</span></span>

|<span data-ttu-id="3a5ad-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3a5ad-116">**Element**</span></span>|<span data-ttu-id="3a5ad-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3a5ad-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a5ad-118">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="3a5ad-118">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="3a5ad-119">Contém o status e o resultado de uma única solicitação de [operação FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="3a5ad-119">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3a5ad-120">Text value</span><span class="sxs-lookup"><span data-stu-id="3a5ad-120">Text value</span></span>

<span data-ttu-id="3a5ad-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3a5ad-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3a5ad-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="3a5ad-122">Remarks</span></span>

<span data-ttu-id="3a5ad-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3a5ad-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a5ad-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3a5ad-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a5ad-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="3a5ad-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3a5ad-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3a5ad-126">Schema Name</span></span>  <br/> |<span data-ttu-id="3a5ad-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="3a5ad-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3a5ad-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3a5ad-128">Validation File</span></span>  <br/> |<span data-ttu-id="3a5ad-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3a5ad-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3a5ad-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3a5ad-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="3a5ad-131">False</span><span class="sxs-lookup"><span data-stu-id="3a5ad-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3a5ad-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="3a5ad-132">See also</span></span>



- [<span data-ttu-id="3a5ad-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3a5ad-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

