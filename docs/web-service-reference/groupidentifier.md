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
description: O elemento GroupIdentifier representa um único identificador de segurança e atributo para um grupo de objetos de serviço de diretório do Active Directory do qual a conta é membro.
ms.openlocfilehash: 8b427b9228cc5e66f46f70389acf2fa4bcd283b3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530800"
---
# <a name="groupidentifier"></a><span data-ttu-id="92b75-103">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="92b75-103">GroupIdentifier</span></span>

<span data-ttu-id="92b75-104">O elemento **GroupIdentifier** representa um único identificador de segurança e atributo para um grupo de objetos de serviço de diretório do Active Directory do qual a conta é membro.</span><span class="sxs-lookup"><span data-stu-id="92b75-104">The **GroupIdentifier** element represents a single security identifier and attribute for an Active Directory directory service object group of which the account is a member.</span></span> 
  
```xml
<GroupIdentifier>
   <SecurityIdentifier/>
</GroupIdentifier>
```

 <span data-ttu-id="92b75-105">**SidAndAttributesType**</span><span class="sxs-lookup"><span data-stu-id="92b75-105">**SidAndAttributesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="92b75-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="92b75-106">Attributes and elements</span></span>

<span data-ttu-id="92b75-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="92b75-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92b75-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="92b75-108">Attributes</span></span>

|<span data-ttu-id="92b75-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="92b75-109">**Attribute**</span></span>|<span data-ttu-id="92b75-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="92b75-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="92b75-111">**Atributos**</span><span class="sxs-lookup"><span data-stu-id="92b75-111">**Attributes**</span></span> <br/> |<span data-ttu-id="92b75-112">Contém atributos de grupo.</span><span class="sxs-lookup"><span data-stu-id="92b75-112">Contains group attributes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="92b75-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="92b75-113">Child elements</span></span>

|<span data-ttu-id="92b75-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="92b75-114">**Element**</span></span>|<span data-ttu-id="92b75-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="92b75-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92b75-116">SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="92b75-116">SecurityIdentifier</span></span>](securityidentifier.md) <br/> |<span data-ttu-id="92b75-117">Representa a forma SDDL (Security Descriptor Definition Language) de um identificador de segurança ([Sid](sid.md)) que representa o grupo.</span><span class="sxs-lookup"><span data-stu-id="92b75-117">Represents the security descriptor definition language (SDDL) form of a security identifier ([SID](sid.md)) that represents the group.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="92b75-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="92b75-118">Parent elements</span></span>

|<span data-ttu-id="92b75-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="92b75-119">**Element**</span></span>|<span data-ttu-id="92b75-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="92b75-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92b75-121">GroupSids</span><span class="sxs-lookup"><span data-stu-id="92b75-121">GroupSids</span></span>](groupsids.md) <br/> |<span data-ttu-id="92b75-122">Representa uma coleção de identificadores de segurança do objeto do grupo do Active Directory que compõem um token de conta para serialização de token.</span><span class="sxs-lookup"><span data-stu-id="92b75-122">Represents a collection of Active Directory group object security identifiers that make up an account token for token serialization.</span></span> <span data-ttu-id="92b75-123">Não há suporte para serialização de token.</span><span class="sxs-lookup"><span data-stu-id="92b75-123">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="92b75-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="92b75-124">Remarks</span></span>

<span data-ttu-id="92b75-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="92b75-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92b75-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="92b75-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92b75-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="92b75-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="92b75-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="92b75-128">Schema Name</span></span>  <br/> |<span data-ttu-id="92b75-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="92b75-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="92b75-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="92b75-130">Validation File</span></span>  <br/> |<span data-ttu-id="92b75-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="92b75-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="92b75-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="92b75-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="92b75-133">False</span><span class="sxs-lookup"><span data-stu-id="92b75-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="92b75-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="92b75-134">See also</span></span>



- [<span data-ttu-id="92b75-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="92b75-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

