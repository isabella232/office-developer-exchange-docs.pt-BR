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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824434"
---
# <a name="member"></a><span data-ttu-id="9d4e7-103">Membro</span><span class="sxs-lookup"><span data-stu-id="9d4e7-103">Member</span></span>

<span data-ttu-id="9d4e7-104">O elemento de **membro** representa um membro de uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="9d4e7-104">The **Member** element represents a member of a distribution list.</span></span> 
  
```xml
<Member Key="">
   <Mailbox/>
   <Status/>
</Member>
```

<span data-ttu-id="9d4e7-105">**MemberType**</span><span class="sxs-lookup"><span data-stu-id="9d4e7-105">**MemberType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9d4e7-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9d4e7-106">Attributes and elements</span></span>

<span data-ttu-id="9d4e7-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9d4e7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d4e7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9d4e7-108">Attributes</span></span>

|<span data-ttu-id="9d4e7-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="9d4e7-109">**Attribute**</span></span>|<span data-ttu-id="9d4e7-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9d4e7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9d4e7-111">Tecla</span><span class="sxs-lookup"><span data-stu-id="9d4e7-111">Key</span></span>  <br/> |<span data-ttu-id="9d4e7-112">Fornece um identificador exclusivo para o membro da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="9d4e7-112">Provides a unique identifier for the distribution list member.</span></span> <span data-ttu-id="9d4e7-113">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="9d4e7-113">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9d4e7-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9d4e7-114">Child elements</span></span>

|<span data-ttu-id="9d4e7-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9d4e7-115">**Element**</span></span>|<span data-ttu-id="9d4e7-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9d4e7-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d4e7-117">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="9d4e7-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="9d4e7-118">Representa o endereço de email do membro da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="9d4e7-118">Represents the e-mail address of the distribution list member.</span></span> <span data-ttu-id="9d4e7-119">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="9d4e7-119">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9d4e7-120">Status (MemberStatusType)</span><span class="sxs-lookup"><span data-stu-id="9d4e7-120">Status (MemberStatusType)</span></span>](status-memberstatustype.md) <br/> |<span data-ttu-id="9d4e7-121">Fornece informações sobre o status de um membro da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="9d4e7-121">Provides information about the status of a distribution list member.</span></span> <span data-ttu-id="9d4e7-122">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="9d4e7-122">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9d4e7-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9d4e7-123">Parent elements</span></span>

|<span data-ttu-id="9d4e7-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9d4e7-124">**Element**</span></span>|<span data-ttu-id="9d4e7-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9d4e7-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d4e7-126">Membros (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="9d4e7-126">Members (MemberListType)</span></span>](members-memberlisttype.md) <br/> |<span data-ttu-id="9d4e7-127">Contém uma lista de membros da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="9d4e7-127">Contains a list of distribution list members.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9d4e7-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="9d4e7-128">Remarks</span></span>

<span data-ttu-id="9d4e7-129">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d4e7-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d4e7-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9d4e7-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d4e7-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="9d4e7-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9d4e7-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9d4e7-132">Schema Name</span></span>  <br/> |<span data-ttu-id="9d4e7-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9d4e7-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="9d4e7-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9d4e7-134">Validation File</span></span>  <br/> |<span data-ttu-id="9d4e7-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9d4e7-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9d4e7-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9d4e7-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d4e7-137">False</span><span class="sxs-lookup"><span data-stu-id="9d4e7-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d4e7-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="9d4e7-138">See also</span></span>

- [<span data-ttu-id="9d4e7-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9d4e7-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

