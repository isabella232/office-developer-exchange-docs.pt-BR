---
title: Destinatários
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 20ef18c2-daa0-4f65-a515-e84e9993a77f
description: O elemento destinatários especifica as pessoas a quem uma tarefa é atribuída.
ms.openlocfilehash: 3e98273e859dbe2128b0ad3b4df42c8016fd3bc5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464711"
---
# <a name="assignees"></a><span data-ttu-id="673b4-103">Destinatários</span><span class="sxs-lookup"><span data-stu-id="673b4-103">Assignees</span></span>

<span data-ttu-id="673b4-104">O elemento **destinatários** especifica as pessoas a quem uma tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="673b4-104">The **Assignees** element specifies the people to whom a task is assigned.</span></span> 
  
```XML
<Assignees>
    <Name></Name>
    <UserID></UserID>
</Assignees>
```

 <span data-ttu-id="673b4-105">**EmailUserType**</span><span class="sxs-lookup"><span data-stu-id="673b4-105">**EmailUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="673b4-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="673b4-106">Attributes and elements</span></span>

<span data-ttu-id="673b4-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="673b4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="673b4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="673b4-108">Attributes</span></span>

<span data-ttu-id="673b4-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="673b4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="673b4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="673b4-110">Child elements</span></span>

|<span data-ttu-id="673b4-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="673b4-111">**Element**</span></span>|<span data-ttu-id="673b4-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="673b4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="673b4-113">Nome (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="673b4-113">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="673b4-114">Representa o nome de exibição do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="673b4-114">Represents the display name of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="673b4-115">UserId (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="673b4-115">UserId (string)</span></span>](userid-string.md) <br/> |<span data-ttu-id="673b4-116">Especifica o identificador de usuário de um usuário de email.</span><span class="sxs-lookup"><span data-stu-id="673b4-116">Specifies the user identifier of an email user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="673b4-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="673b4-117">Parent elements</span></span>

|<span data-ttu-id="673b4-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="673b4-118">**Element**</span></span>|<span data-ttu-id="673b4-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="673b4-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="673b4-120">TaskSuggestion</span><span class="sxs-lookup"><span data-stu-id="673b4-120">TaskSuggestion</span></span>](tasksuggestion.md) <br/> |<span data-ttu-id="673b4-121">Especifica uma tarefa proposta.</span><span class="sxs-lookup"><span data-stu-id="673b4-121">Specifies a proposed task.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="673b4-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="673b4-122">Remarks</span></span>

<span data-ttu-id="673b4-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="673b4-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="673b4-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="673b4-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="673b4-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="673b4-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="673b4-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="673b4-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="673b4-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="673b4-127">Schema Name</span></span>  <br/> |<span data-ttu-id="673b4-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="673b4-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="673b4-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="673b4-129">Validation File</span></span>  <br/> |<span data-ttu-id="673b4-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="673b4-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="673b4-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="673b4-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="673b4-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="673b4-132">See also</span></span>

- [<span data-ttu-id="673b4-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="673b4-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

