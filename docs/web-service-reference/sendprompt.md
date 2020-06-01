---
title: SendPrompt
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22cb5a30-75d9-49a8-9d98-255f2e8a722d
description: O elemento SendPrompt especifica o tipo de ação permitida para uma opção de votação.
ms.openlocfilehash: 98ffc69cdc94c3f7b9c325bee0c1ebaeb407ee96
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462098"
---
# <a name="sendprompt"></a><span data-ttu-id="ab8de-103">SendPrompt</span><span class="sxs-lookup"><span data-stu-id="ab8de-103">SendPrompt</span></span>

<span data-ttu-id="ab8de-104">O elemento **SendPrompt** especifica o tipo de ação permitida para uma opção de votação.</span><span class="sxs-lookup"><span data-stu-id="ab8de-104">The **SendPrompt** element specifies the type of action allowed for a voting option.</span></span> 
  
```XML
<SendPrompt> None | Send | VotingOption </SendPrompt>
```

 <span data-ttu-id="ab8de-105">**SendPromptType**</span><span class="sxs-lookup"><span data-stu-id="ab8de-105">**SendPromptType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ab8de-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ab8de-106">Attributes and elements</span></span>

<span data-ttu-id="ab8de-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ab8de-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ab8de-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ab8de-108">Attributes</span></span>

<span data-ttu-id="ab8de-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ab8de-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ab8de-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ab8de-110">Child elements</span></span>

<span data-ttu-id="ab8de-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ab8de-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ab8de-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ab8de-112">Parent elements</span></span>

[<span data-ttu-id="ab8de-113">VotingOptionData</span><span class="sxs-lookup"><span data-stu-id="ab8de-113">VotingOptionData</span></span>](votingoptiondata.md)
  
## <a name="text-value"></a><span data-ttu-id="ab8de-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="ab8de-114">Text value</span></span>

<span data-ttu-id="ab8de-115">O valor de texto do elemento **SendPrompt** é uma ação de opção de votação.</span><span class="sxs-lookup"><span data-stu-id="ab8de-115">The text value of the **SendPrompt** element is a voting option action.</span></span> <span data-ttu-id="ab8de-116">A tabela a seguir lista os valores possíveis para este elemento.</span><span class="sxs-lookup"><span data-stu-id="ab8de-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="ab8de-117">**Valor**</span><span class="sxs-lookup"><span data-stu-id="ab8de-117">**Value**</span></span>|<span data-ttu-id="ab8de-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ab8de-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ab8de-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ab8de-119">None</span></span>  <br/> |<span data-ttu-id="ab8de-120">Nenhuma ação.</span><span class="sxs-lookup"><span data-stu-id="ab8de-120">No action.</span></span>  <br/> |
|<span data-ttu-id="ab8de-121">Enviar</span><span class="sxs-lookup"><span data-stu-id="ab8de-121">Send</span></span>  <br/> |<span data-ttu-id="ab8de-122">A resposta é enviada imediatamente.</span><span class="sxs-lookup"><span data-stu-id="ab8de-122">The response is sent immediately.</span></span>  <br/> |
|<span data-ttu-id="ab8de-123">VotingOption</span><span class="sxs-lookup"><span data-stu-id="ab8de-123">VotingOption</span></span>  <br/> |<span data-ttu-id="ab8de-124">O aprovador pode inserir comentários ao aprovar ou rejeitar.</span><span class="sxs-lookup"><span data-stu-id="ab8de-124">The approver can enter comments while approving or rejecting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ab8de-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="ab8de-125">Remarks</span></span>

<span data-ttu-id="ab8de-126">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ab8de-126">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="ab8de-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab8de-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ab8de-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ab8de-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ab8de-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="ab8de-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ab8de-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ab8de-130">Schema Name</span></span>  <br/> |<span data-ttu-id="ab8de-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ab8de-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="ab8de-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ab8de-132">Validation File</span></span>  <br/> |<span data-ttu-id="ab8de-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ab8de-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ab8de-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ab8de-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="ab8de-135">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="ab8de-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ab8de-136">Também consulte</span><span class="sxs-lookup"><span data-stu-id="ab8de-136">See also</span></span>



[<span data-ttu-id="ab8de-137">VotingOptionData</span><span class="sxs-lookup"><span data-stu-id="ab8de-137">VotingOptionData</span></span>](votingoptiondata.md)


- [<span data-ttu-id="ab8de-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ab8de-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

