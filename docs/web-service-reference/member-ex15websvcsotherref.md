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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824434"
---
# <a name="member"></a><span data-ttu-id="8be17-103">Membro</span><span class="sxs-lookup"><span data-stu-id="8be17-103">Member</span></span>

<span data-ttu-id="8be17-104">O elemento de **membro** representa um membro de uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="8be17-104">The **Member** element represents a member of a distribution list.</span></span> 
  
```xml
<Member Key="">
   <Mailbox/>
   <Status/>
</Member>
```

<span data-ttu-id="8be17-105">**MemberType**</span><span class="sxs-lookup"><span data-stu-id="8be17-105">**MemberType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8be17-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8be17-106">Attributes and elements</span></span>

<span data-ttu-id="8be17-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8be17-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8be17-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8be17-108">Attributes</span></span>

|<span data-ttu-id="8be17-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="8be17-109">**Attribute**</span></span>|<span data-ttu-id="8be17-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8be17-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8be17-111">Tecla</span><span class="sxs-lookup"><span data-stu-id="8be17-111">Key</span></span>  <br/> |<span data-ttu-id="8be17-112">Fornece um identificador exclusivo para o membro da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="8be17-112">Provides a unique identifier for the distribution list member.</span></span> <span data-ttu-id="8be17-113">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="8be17-113">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8be17-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8be17-114">Child elements</span></span>

|<span data-ttu-id="8be17-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8be17-115">**Element**</span></span>|<span data-ttu-id="8be17-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8be17-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8be17-117">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="8be17-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="8be17-118">Representa o endereço de email do membro da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="8be17-118">Represents the e-mail address of the distribution list member.</span></span> <span data-ttu-id="8be17-119">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="8be17-119">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8be17-120">Status (MemberStatusType)</span><span class="sxs-lookup"><span data-stu-id="8be17-120">Status (MemberStatusType)</span></span>](status-memberstatustype.md) <br/> |<span data-ttu-id="8be17-121">Fornece informações sobre o status de um membro da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="8be17-121">Provides information about the status of a distribution list member.</span></span> <span data-ttu-id="8be17-122">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="8be17-122">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8be17-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8be17-123">Parent elements</span></span>

|<span data-ttu-id="8be17-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8be17-124">**Element**</span></span>|<span data-ttu-id="8be17-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8be17-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8be17-126">Membros (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="8be17-126">Members (MemberListType)</span></span>](members-memberlisttype.md) <br/> |<span data-ttu-id="8be17-127">Contém uma lista de membros da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="8be17-127">Contains a list of distribution list members.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8be17-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="8be17-128">Remarks</span></span>

<span data-ttu-id="8be17-129">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8be17-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8be17-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8be17-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8be17-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="8be17-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8be17-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8be17-132">Schema Name</span></span>  <br/> |<span data-ttu-id="8be17-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8be17-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="8be17-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8be17-134">Validation File</span></span>  <br/> |<span data-ttu-id="8be17-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8be17-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8be17-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8be17-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="8be17-137">False</span><span class="sxs-lookup"><span data-stu-id="8be17-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8be17-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="8be17-138">See also</span></span>

- [<span data-ttu-id="8be17-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8be17-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

