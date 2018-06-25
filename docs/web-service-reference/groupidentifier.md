---
title: GroupIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupIdentifier
api_type:
- schema
ms.assetid: bdc6fc1e-4979-42da-a35b-e3017988c7d3
description: O elemento GroupIdentifier representa um identificador de segurança único e o atributo para um grupo de objetos do Active Directory directory service do qual a conta é membro.
ms.openlocfilehash: d73d72979762238ca09496cfbd6636b4ff44a969
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823767"
---
# <a name="groupidentifier"></a><span data-ttu-id="bc044-103">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="bc044-103">GroupIdentifier</span></span>

<span data-ttu-id="bc044-104">O elemento **GroupIdentifier** representa um identificador de segurança único e o atributo para um grupo de objetos do Active Directory directory service do qual a conta é membro.</span><span class="sxs-lookup"><span data-stu-id="bc044-104">The **GroupIdentifier** element represents a single security identifier and attribute for an Active Directory directory service object group of which the account is a member.</span></span> 
  
```xml
<GroupIdentifier>
   <SecurityIdentifier/>
</GroupIdentifier>
```

 <span data-ttu-id="bc044-105">**SidAndAttributesType**</span><span class="sxs-lookup"><span data-stu-id="bc044-105">**SidAndAttributesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc044-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="bc044-106">Attributes and elements</span></span>

<span data-ttu-id="bc044-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bc044-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc044-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="bc044-108">Attributes</span></span>

|<span data-ttu-id="bc044-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="bc044-109">**Attribute**</span></span>|<span data-ttu-id="bc044-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bc044-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bc044-111">**Attributes**</span><span class="sxs-lookup"><span data-stu-id="bc044-111">**Attributes**</span></span> <br/> |<span data-ttu-id="bc044-112">Contém atributos de grupo.</span><span class="sxs-lookup"><span data-stu-id="bc044-112">Contains group attributes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bc044-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bc044-113">Child elements</span></span>

|<span data-ttu-id="bc044-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bc044-114">**Element**</span></span>|<span data-ttu-id="bc044-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bc044-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc044-116">SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="bc044-116">SecurityIdentifier</span></span>](securityidentifier.md) <br/> |<span data-ttu-id="bc044-117">Representa o formulário de segurança descritor definition language (SDDL) de um identificador de segurança ([SID](sid.md)) que representa o grupo.</span><span class="sxs-lookup"><span data-stu-id="bc044-117">Represents the security descriptor definition language (SDDL) form of a security identifier ([SID](sid.md)) that represents the group.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bc044-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bc044-118">Parent elements</span></span>

|<span data-ttu-id="bc044-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bc044-119">**Element**</span></span>|<span data-ttu-id="bc044-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bc044-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc044-121">GroupSids</span><span class="sxs-lookup"><span data-stu-id="bc044-121">GroupSids</span></span>](groupsids.md) <br/> |<span data-ttu-id="bc044-122">Representa uma coleção de identificadores segurança de objeto de grupo de Active Directory que compõem um token de conta para serialização de token.</span><span class="sxs-lookup"><span data-stu-id="bc044-122">Represents a collection of Active Directory group object security identifiers that make up an account token for token serialization.</span></span> <span data-ttu-id="bc044-123">Serialização de token não é suportada.</span><span class="sxs-lookup"><span data-stu-id="bc044-123">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bc044-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="bc044-124">Remarks</span></span>

<span data-ttu-id="bc044-125">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="bc044-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc044-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="bc044-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc044-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="bc044-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bc044-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="bc044-128">Schema Name</span></span>  <br/> |<span data-ttu-id="bc044-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="bc044-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="bc044-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="bc044-130">Validation File</span></span>  <br/> |<span data-ttu-id="bc044-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bc044-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bc044-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="bc044-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc044-133">False</span><span class="sxs-lookup"><span data-stu-id="bc044-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc044-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="bc044-134">See also</span></span>



- [<span data-ttu-id="bc044-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="bc044-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

