---
title: FailedMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f34fb6f6-057e-4ae3-8e10-bc92112eafba
description: O elemento FailedMailboxes especifica uma matriz de caixas de correio que falharam na pesquisa.
ms.openlocfilehash: 10f10d3f2ac4379d7ddcb3a13019d17a17bb676a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461951"
---
# <a name="failedmailboxes"></a><span data-ttu-id="4b49f-103">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="4b49f-103">FailedMailboxes</span></span>

<span data-ttu-id="4b49f-104">O elemento **FailedMailboxes** especifica uma matriz de caixas de correio que falharam na pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4b49f-104">The **FailedMailboxes** element specifies an array of mailboxes that failed on search.</span></span> 
  
```XML
<FailedMailboxes>
    <FailedMailbox/>
<FailedMailboxes>
```

 <span data-ttu-id="4b49f-105">**ArrayOfFailedSearchMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="4b49f-105">**ArrayOfFailedSearchMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4b49f-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4b49f-106">Attributes and elements</span></span>

<span data-ttu-id="4b49f-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4b49f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b49f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4b49f-108">Attributes</span></span>

<span data-ttu-id="4b49f-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4b49f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4b49f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4b49f-110">Child elements</span></span>

|<span data-ttu-id="4b49f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4b49f-111">**Element**</span></span>|<span data-ttu-id="4b49f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4b49f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b49f-113">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="4b49f-113">FailedMailbox</span></span>](failedmailbox.md) <br/> |<span data-ttu-id="4b49f-114">Especifica a mensagem de erro para uma caixa de correio que falhou na pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4b49f-114">Specifies the error message for a mailbox that failed on search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4b49f-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4b49f-115">Parent elements</span></span>

|<span data-ttu-id="4b49f-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4b49f-116">**Element**</span></span>|<span data-ttu-id="4b49f-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4b49f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b49f-118">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="4b49f-118">SearchMailboxesResult</span></span>](searchmailboxesresult.md) <br/> |<span data-ttu-id="4b49f-119">Contém o resultado da solicitação **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="4b49f-119">Contains the result of the **SearchMailboxes** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4b49f-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="4b49f-120">Remarks</span></span>

<span data-ttu-id="4b49f-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4b49f-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4b49f-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b49f-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4b49f-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4b49f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b49f-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="4b49f-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4b49f-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4b49f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4b49f-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="4b49f-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="4b49f-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4b49f-127">Validation File</span></span>  <br/> |<span data-ttu-id="4b49f-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4b49f-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4b49f-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="4b49f-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4b49f-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="4b49f-130">See also</span></span>



- [<span data-ttu-id="4b49f-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4b49f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

