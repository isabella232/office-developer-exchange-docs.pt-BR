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
ms.openlocfilehash: 1e03cb135b7b2a125da1e29f7293d233f4e20ddb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468674"
---
# <a name="messagetrackingsearchresults"></a><span data-ttu-id="c1e3a-103">MessageTrackingSearchResults</span><span class="sxs-lookup"><span data-stu-id="c1e3a-103">MessageTrackingSearchResults</span></span>

<span data-ttu-id="c1e3a-104">O elemento **MessageTrackingSearchResults** contém uma lista de registros que correspondem aos critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c1e3a-104">The **MessageTrackingSearchResults** element contains a list of records that match the search criteria.</span></span> 
  
```XML
<MessageTrackingSearchResults>
   <MessageTrackingSearchResult/>
</MessageTrackingSearchResults>
```

 <span data-ttu-id="c1e3a-105">**ArrayOfFindMessageTrackingSearchResultType**</span><span class="sxs-lookup"><span data-stu-id="c1e3a-105">**ArrayOfFindMessageTrackingSearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c1e3a-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c1e3a-106">Attributes and elements</span></span>

<span data-ttu-id="c1e3a-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c1e3a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c1e3a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c1e3a-108">Attributes</span></span>

<span data-ttu-id="c1e3a-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c1e3a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c1e3a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c1e3a-110">Child elements</span></span>

|<span data-ttu-id="c1e3a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c1e3a-111">**Element**</span></span>|<span data-ttu-id="c1e3a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c1e3a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1e3a-113">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="c1e3a-113">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="c1e3a-114">Contém um único resultado de mensagem para um elemento [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="c1e3a-114">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c1e3a-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c1e3a-115">Parent elements</span></span>

|<span data-ttu-id="c1e3a-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c1e3a-116">**Element**</span></span>|<span data-ttu-id="c1e3a-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c1e3a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1e3a-118">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="c1e3a-118">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="c1e3a-119">Contém o status e o resultado de uma única solicitação de [operação FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="c1e3a-119">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c1e3a-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c1e3a-120">Text value</span></span>

<span data-ttu-id="c1e3a-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c1e3a-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c1e3a-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="c1e3a-122">Remarks</span></span>

<span data-ttu-id="c1e3a-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1e3a-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c1e3a-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c1e3a-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c1e3a-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="c1e3a-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c1e3a-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c1e3a-126">Schema Name</span></span>  <br/> |<span data-ttu-id="c1e3a-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c1e3a-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c1e3a-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c1e3a-128">Validation File</span></span>  <br/> |<span data-ttu-id="c1e3a-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c1e3a-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c1e3a-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c1e3a-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="c1e3a-131">False</span><span class="sxs-lookup"><span data-stu-id="c1e3a-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c1e3a-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="c1e3a-132">See also</span></span>



- [<span data-ttu-id="c1e3a-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c1e3a-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

