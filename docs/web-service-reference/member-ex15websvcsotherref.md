---
title: Membro
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Member
api_type:
- schema
ms.assetid: af9c5ff8-02a4-41fc-876d-14ac05f1ee77
description: O elemento de membro representa um membro de uma lista de distribuição.
ms.openlocfilehash: c38e2ed24e78b5199d4d65cce27a00a8e6704037
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/21/2018
ms.locfileid: "19824434"
---
# <a name="member"></a><span data-ttu-id="ea542-103">Membro</span><span class="sxs-lookup"><span data-stu-id="ea542-103">Member</span></span>

<span data-ttu-id="ea542-104">O elemento de **membro** representa um membro de uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="ea542-104">The **Member** element represents a member of a distribution list.</span></span> 
  
```xml
<Member Key="">
   <Mailbox/>
   <Status/>
</Member>
```

<span data-ttu-id="ea542-105">**MemberType**</span><span class="sxs-lookup"><span data-stu-id="ea542-105">**MemberType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ea542-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ea542-106">Attributes and elements</span></span>

<span data-ttu-id="ea542-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ea542-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea542-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ea542-108">Attributes</span></span>

|<span data-ttu-id="ea542-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="ea542-109">**Attribute**</span></span>|<span data-ttu-id="ea542-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ea542-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ea542-111">Tecla</span><span class="sxs-lookup"><span data-stu-id="ea542-111">Key</span></span>  <br/> |<span data-ttu-id="ea542-112">Fornece um identificador exclusivo para o membro da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="ea542-112">Provides a unique identifier for the distribution list member.</span></span> <span data-ttu-id="ea542-113">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="ea542-113">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ea542-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ea542-114">Child elements</span></span>

|<span data-ttu-id="ea542-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ea542-115">**Element**</span></span>|<span data-ttu-id="ea542-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ea542-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea542-117">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="ea542-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="ea542-118">Representa o endereço de email do membro da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="ea542-118">Represents the e-mail address of the distribution list member.</span></span> <span data-ttu-id="ea542-119">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="ea542-119">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ea542-120">Status (MemberStatusType)</span><span class="sxs-lookup"><span data-stu-id="ea542-120">Status (MemberStatusType)</span></span>](status-memberstatustype.md) <br/> |<span data-ttu-id="ea542-121">Fornece informações sobre o status de um membro da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="ea542-121">Provides information about the status of a distribution list member.</span></span> <span data-ttu-id="ea542-122">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="ea542-122">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ea542-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ea542-123">Parent elements</span></span>

|<span data-ttu-id="ea542-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ea542-124">**Element**</span></span>|<span data-ttu-id="ea542-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ea542-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea542-126">Membros (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="ea542-126">Members (MemberListType)</span></span>](members-memberlisttype.md) <br/> |<span data-ttu-id="ea542-127">Contém uma lista de membros da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="ea542-127">Contains a list of distribution list members.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ea542-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="ea542-128">Remarks</span></span>

<span data-ttu-id="ea542-129">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ea542-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ea542-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ea542-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea542-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="ea542-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ea542-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ea542-132">Schema Name</span></span>  <br/> |<span data-ttu-id="ea542-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ea542-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="ea542-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ea542-134">Validation File</span></span>  <br/> |<span data-ttu-id="ea542-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ea542-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ea542-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ea542-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="ea542-137">False</span><span class="sxs-lookup"><span data-stu-id="ea542-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ea542-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="ea542-138">See also</span></span>

- [<span data-ttu-id="ea542-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ea542-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

