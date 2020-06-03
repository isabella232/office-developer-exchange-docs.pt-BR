---
title: FindMailboxStatisticsByKeywordsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: af1dd9bf-df47-473d-a2ce-ab9a01a37606
description: O elemento FindMailboxStatisticsByKeywordsResponse especifica a resposta a uma solicitação FindMailboxStatisticsByKeywords.
ms.openlocfilehash: a0595ec9ee0cedf5150852dc39eca50b598e15aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460985"
---
# <a name="findmailboxstatisticsbykeywordsresponse"></a><span data-ttu-id="1dc25-103">FindMailboxStatisticsByKeywordsResponse</span><span class="sxs-lookup"><span data-stu-id="1dc25-103">FindMailboxStatisticsByKeywordsResponse</span></span>

<span data-ttu-id="1dc25-104">O elemento **FindMailboxStatisticsByKeywordsResponse** especifica a resposta a uma solicitação **FindMailboxStatisticsByKeywords** .</span><span class="sxs-lookup"><span data-stu-id="1dc25-104">The **FindMailboxStatisticsByKeywordsResponse** element specifies the response to a **FindMailboxStatisticsByKeywords** request.</span></span> 
  
```XML
<FindMailboxStatisticsByKeywordsResponse>
    <ResponseMessages/>
</FindMailboxStatisticsByKeywordsResponse>
```

 <span data-ttu-id="1dc25-105">**FindMailboxStatisticsByKeywordsResponseType**</span><span class="sxs-lookup"><span data-stu-id="1dc25-105">**FindMailboxStatisticsByKeywordsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1dc25-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1dc25-106">Attributes and elements</span></span>

<span data-ttu-id="1dc25-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1dc25-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1dc25-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1dc25-108">Attributes</span></span>

<span data-ttu-id="1dc25-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1dc25-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1dc25-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1dc25-110">Child elements</span></span>

|<span data-ttu-id="1dc25-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1dc25-111">**Element**</span></span>|<span data-ttu-id="1dc25-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1dc25-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1dc25-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1dc25-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="1dc25-114">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="1dc25-114">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1dc25-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1dc25-115">Parent elements</span></span>

<span data-ttu-id="1dc25-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1dc25-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1dc25-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="1dc25-117">Remarks</span></span>

<span data-ttu-id="1dc25-118">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1dc25-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1dc25-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1dc25-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1dc25-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="1dc25-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1dc25-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1dc25-121">Schema Name</span></span>  <br/> |<span data-ttu-id="1dc25-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="1dc25-122">Message schema</span></span>  <br/> |
|<span data-ttu-id="1dc25-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1dc25-123">Validation File</span></span>  <br/> |<span data-ttu-id="1dc25-124">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1dc25-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1dc25-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="1dc25-125">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1dc25-126">Confira também</span><span class="sxs-lookup"><span data-stu-id="1dc25-126">See also</span></span>



- [<span data-ttu-id="1dc25-127">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1dc25-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

