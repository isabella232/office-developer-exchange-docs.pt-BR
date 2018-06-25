---
title: Destinatários
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 20ef18c2-daa0-4f65-a515-e84e9993a77f
description: O elemento os destinatários Especifica as pessoas a quem uma tarefa for atribuída.
ms.openlocfilehash: 5fc301cd77268213e95fd33a2a2f36dbe218b512
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751211"
---
# <a name="assignees"></a><span data-ttu-id="74a2d-103">Destinatários</span><span class="sxs-lookup"><span data-stu-id="74a2d-103">Assignees</span></span>

<span data-ttu-id="74a2d-104">**Os destinatários de** elemento Especifica as pessoas a quem uma tarefa for atribuída.</span><span class="sxs-lookup"><span data-stu-id="74a2d-104">The **Assignees** element specifies the people to whom a task is assigned.</span></span> 
  
```XML
<Assignees>
    <Name></Name>
    <UserID></UserID>
</Assignees>
```

 <span data-ttu-id="74a2d-105">**EmailUserType**</span><span class="sxs-lookup"><span data-stu-id="74a2d-105">**EmailUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74a2d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="74a2d-106">Attributes and elements</span></span>

<span data-ttu-id="74a2d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="74a2d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74a2d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="74a2d-108">Attributes</span></span>

<span data-ttu-id="74a2d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="74a2d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74a2d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="74a2d-110">Child elements</span></span>

|<span data-ttu-id="74a2d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="74a2d-111">**Element**</span></span>|<span data-ttu-id="74a2d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="74a2d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74a2d-113">Nome (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="74a2d-113">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="74a2d-114">Representa o nome de exibição do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="74a2d-114">Represents the display name of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="74a2d-115">UserId (string)</span><span class="sxs-lookup"><span data-stu-id="74a2d-115">UserId (string)</span></span>](userid-string.md) <br/> |<span data-ttu-id="74a2d-116">Especifica o identificador de usuário de um usuário de email.</span><span class="sxs-lookup"><span data-stu-id="74a2d-116">Specifies the user identifier of an email user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="74a2d-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="74a2d-117">Parent elements</span></span>

|<span data-ttu-id="74a2d-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="74a2d-118">**Element**</span></span>|<span data-ttu-id="74a2d-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="74a2d-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74a2d-120">TaskSuggestion</span><span class="sxs-lookup"><span data-stu-id="74a2d-120">TaskSuggestion</span></span>](tasksuggestion.md) <br/> |<span data-ttu-id="74a2d-121">Especifica uma tarefa da proposta.</span><span class="sxs-lookup"><span data-stu-id="74a2d-121">Specifies a proposed task.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="74a2d-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="74a2d-122">Remarks</span></span>

<span data-ttu-id="74a2d-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="74a2d-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="74a2d-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="74a2d-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74a2d-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="74a2d-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74a2d-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="74a2d-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="74a2d-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="74a2d-127">Schema Name</span></span>  <br/> |<span data-ttu-id="74a2d-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="74a2d-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="74a2d-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="74a2d-129">Validation File</span></span>  <br/> |<span data-ttu-id="74a2d-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="74a2d-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="74a2d-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="74a2d-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="74a2d-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="74a2d-132">See also</span></span>

- [<span data-ttu-id="74a2d-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="74a2d-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

