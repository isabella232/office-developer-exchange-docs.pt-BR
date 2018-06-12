---
title: SendPrompt
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22cb5a30-75d9-49a8-9d98-255f2e8a722d
description: O elemento SendPrompt Especifica o tipo de ação permitida para uma opção de votação.
ms.openlocfilehash: f3220d957482ea04c46b014cdf1c67025d5ec21a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825346"
---
# <a name="sendprompt"></a><span data-ttu-id="3f3ab-103">SendPrompt</span><span class="sxs-lookup"><span data-stu-id="3f3ab-103">SendPrompt</span></span>

<span data-ttu-id="3f3ab-104">O elemento **SendPrompt** Especifica o tipo de ação permitida para uma opção de votação.</span><span class="sxs-lookup"><span data-stu-id="3f3ab-104">The **SendPrompt** element specifies the type of action allowed for a voting option.</span></span> 
  
```XML
<SendPrompt> None | Send | VotingOption </SendPrompt>
```

 <span data-ttu-id="3f3ab-105">**SendPromptType**</span><span class="sxs-lookup"><span data-stu-id="3f3ab-105">**SendPromptType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3f3ab-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3f3ab-106">Attributes and elements</span></span>

<span data-ttu-id="3f3ab-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3f3ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3f3ab-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3f3ab-108">Attributes</span></span>

<span data-ttu-id="3f3ab-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3f3ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3f3ab-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3f3ab-110">Child elements</span></span>

<span data-ttu-id="3f3ab-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3f3ab-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3f3ab-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3f3ab-112">Parent elements</span></span>

[<span data-ttu-id="3f3ab-113">VotingOptionData</span><span class="sxs-lookup"><span data-stu-id="3f3ab-113">VotingOptionData</span></span>](votingoptiondata.md)
  
## <a name="text-value"></a><span data-ttu-id="3f3ab-114">Text value</span><span class="sxs-lookup"><span data-stu-id="3f3ab-114">Text value</span></span>

<span data-ttu-id="3f3ab-115">O valor de texto do elemento **SendPrompt** é uma ação de opção de votação.</span><span class="sxs-lookup"><span data-stu-id="3f3ab-115">The text value of the **SendPrompt** element is a voting option action.</span></span> <span data-ttu-id="3f3ab-116">A tabela a seguir lista os valores possíveis para esse elemento.</span><span class="sxs-lookup"><span data-stu-id="3f3ab-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="3f3ab-117">**Valor**</span><span class="sxs-lookup"><span data-stu-id="3f3ab-117">**Value**</span></span>|<span data-ttu-id="3f3ab-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3f3ab-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3f3ab-119">None</span><span class="sxs-lookup"><span data-stu-id="3f3ab-119">None</span></span>  <br/> |<span data-ttu-id="3f3ab-120">Nenhuma ação.</span><span class="sxs-lookup"><span data-stu-id="3f3ab-120">No action.</span></span>  <br/> |
|<span data-ttu-id="3f3ab-121">Enviar</span><span class="sxs-lookup"><span data-stu-id="3f3ab-121">Send</span></span>  <br/> |<span data-ttu-id="3f3ab-122">A resposta é enviada imediatamente.</span><span class="sxs-lookup"><span data-stu-id="3f3ab-122">The response is sent immediately.</span></span>  <br/> |
|<span data-ttu-id="3f3ab-123">VotingOption</span><span class="sxs-lookup"><span data-stu-id="3f3ab-123">VotingOption</span></span>  <br/> |<span data-ttu-id="3f3ab-124">O aprovador pode inserir comentários ao aprovar ou rejeitar.</span><span class="sxs-lookup"><span data-stu-id="3f3ab-124">The approver can enter comments while approving or rejecting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3f3ab-125">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="3f3ab-125">Remarks</span></span>

<span data-ttu-id="3f3ab-126">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3f3ab-126">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="3f3ab-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f3ab-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3f3ab-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3f3ab-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3f3ab-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="3f3ab-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3f3ab-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3f3ab-130">Schema Name</span></span>  <br/> |<span data-ttu-id="3f3ab-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3f3ab-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="3f3ab-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3f3ab-132">Validation File</span></span>  <br/> |<span data-ttu-id="3f3ab-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3f3ab-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3f3ab-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3f3ab-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="3f3ab-135">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="3f3ab-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3f3ab-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="3f3ab-136">See also</span></span>



[<span data-ttu-id="3f3ab-137">VotingOptionData</span><span class="sxs-lookup"><span data-stu-id="3f3ab-137">VotingOptionData</span></span>](votingoptiondata.md)


- [<span data-ttu-id="3f3ab-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3f3ab-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

