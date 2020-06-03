---
title: Member
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
description: O elemento member representa um membro de uma lista de distribuição.
ms.openlocfilehash: e84223b7c41846ca2f174293bff46a8825777a0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457302"
---
# <a name="member"></a><span data-ttu-id="aa494-103">Member</span><span class="sxs-lookup"><span data-stu-id="aa494-103">Member</span></span>

<span data-ttu-id="aa494-104">O elemento **Member** representa um membro de uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="aa494-104">The **Member** element represents a member of a distribution list.</span></span> 
  
```xml
<Member Key="">
   <Mailbox/>
   <Status/>
</Member>
```

<span data-ttu-id="aa494-105">**MemberType**</span><span class="sxs-lookup"><span data-stu-id="aa494-105">**MemberType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="aa494-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="aa494-106">Attributes and elements</span></span>

<span data-ttu-id="aa494-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="aa494-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa494-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="aa494-108">Attributes</span></span>

|<span data-ttu-id="aa494-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="aa494-109">**Attribute**</span></span>|<span data-ttu-id="aa494-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aa494-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aa494-111">Chave</span><span class="sxs-lookup"><span data-stu-id="aa494-111">Key</span></span>  <br/> |<span data-ttu-id="aa494-112">Fornece um identificador exclusivo para o membro da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="aa494-112">Provides a unique identifier for the distribution list member.</span></span> <span data-ttu-id="aa494-113">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="aa494-113">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="aa494-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="aa494-114">Child elements</span></span>

|<span data-ttu-id="aa494-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aa494-115">**Element**</span></span>|<span data-ttu-id="aa494-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aa494-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa494-117">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="aa494-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="aa494-118">Representa o endereço de email do membro da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="aa494-118">Represents the e-mail address of the distribution list member.</span></span> <span data-ttu-id="aa494-119">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="aa494-119">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="aa494-120">Status (MemberStatusType)</span><span class="sxs-lookup"><span data-stu-id="aa494-120">Status (MemberStatusType)</span></span>](status-memberstatustype.md) <br/> |<span data-ttu-id="aa494-121">Fornece informações sobre o status de um membro da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="aa494-121">Provides information about the status of a distribution list member.</span></span> <span data-ttu-id="aa494-122">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="aa494-122">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aa494-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="aa494-123">Parent elements</span></span>

|<span data-ttu-id="aa494-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aa494-124">**Element**</span></span>|<span data-ttu-id="aa494-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aa494-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa494-126">Membros (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="aa494-126">Members (MemberListType)</span></span>](members-memberlisttype.md) <br/> |<span data-ttu-id="aa494-127">Contém uma lista de membros da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="aa494-127">Contains a list of distribution list members.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aa494-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="aa494-128">Remarks</span></span>

<span data-ttu-id="aa494-129">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa494-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aa494-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="aa494-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa494-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="aa494-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aa494-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="aa494-132">Schema Name</span></span>  <br/> |<span data-ttu-id="aa494-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="aa494-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="aa494-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="aa494-134">Validation File</span></span>  <br/> |<span data-ttu-id="aa494-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="aa494-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aa494-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="aa494-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="aa494-137">False</span><span class="sxs-lookup"><span data-stu-id="aa494-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aa494-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="aa494-138">See also</span></span>

- [<span data-ttu-id="aa494-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="aa494-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

