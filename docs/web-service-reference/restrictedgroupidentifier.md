---
title: RestrictedGroupIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RestrictedGroupIdentifier
api_type:
- schema
ms.assetid: a3ea3c81-9f99-4836-8cb4-2384ea63f093
description: O elemento RestrictGroupIdentifier representa o identificador de segurança do grupo (SID) e os atributos de um grupo restrito dentro de um token de usuário.
ms.openlocfilehash: c95af4e09324e96f4551a05490dc200aec0cbd46
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465363"
---
# <a name="restrictedgroupidentifier"></a><span data-ttu-id="822a5-103">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="822a5-103">RestrictedGroupIdentifier</span></span>

<span data-ttu-id="822a5-104">O elemento **RestrictGroupIdentifier** representa o identificador de segurança do grupo (SID) e os atributos de um grupo restrito dentro de um token de usuário.</span><span class="sxs-lookup"><span data-stu-id="822a5-104">The **RestrictGroupIdentifier** element represents the group security identifier (SID) and attributes for a restricted group within a user token.</span></span> 
  
```xml
<RestrictedGroupIdentifier Attributes="">
   <SecurityIdentifier/>
</RestrictedGroupIdentifier>
```

 <span data-ttu-id="822a5-105">**SidAndAttributesType**</span><span class="sxs-lookup"><span data-stu-id="822a5-105">**SidAndAttributesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="822a5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="822a5-106">Attributes and elements</span></span>

<span data-ttu-id="822a5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="822a5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="822a5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="822a5-108">Attributes</span></span>

|<span data-ttu-id="822a5-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="822a5-109">**Attribute**</span></span>|<span data-ttu-id="822a5-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="822a5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="822a5-111">**Atributos**</span><span class="sxs-lookup"><span data-stu-id="822a5-111">**Attributes**</span></span> <br/> |<span data-ttu-id="822a5-112">Contém atributos de grupo.</span><span class="sxs-lookup"><span data-stu-id="822a5-112">Contains group attributes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="822a5-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="822a5-113">Child elements</span></span>

|<span data-ttu-id="822a5-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="822a5-114">**Element**</span></span>|<span data-ttu-id="822a5-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="822a5-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="822a5-116">SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="822a5-116">SecurityIdentifier</span></span>](securityidentifier.md) <br/> |<span data-ttu-id="822a5-117">Representa a forma SDDL (Security Descriptor Definition Language) de um identificador de segurança.</span><span class="sxs-lookup"><span data-stu-id="822a5-117">Represents the security descriptor definition language (SDDL) form of a security identifier.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="822a5-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="822a5-118">Parent elements</span></span>

|<span data-ttu-id="822a5-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="822a5-119">**Element**</span></span>|<span data-ttu-id="822a5-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="822a5-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="822a5-121">RestrictedGroupSids</span><span class="sxs-lookup"><span data-stu-id="822a5-121">RestrictedGroupSids</span></span>](restrictedgroupsids.md) <br/> |<span data-ttu-id="822a5-122">Representa uma coleção de grupos restritos dentro de um token de usuário.</span><span class="sxs-lookup"><span data-stu-id="822a5-122">Represents a collection of restricted groups within a user token.</span></span> <span data-ttu-id="822a5-123">Não há suporte para serialização de token.</span><span class="sxs-lookup"><span data-stu-id="822a5-123">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="822a5-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="822a5-124">Remarks</span></span>

<span data-ttu-id="822a5-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="822a5-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="822a5-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="822a5-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="822a5-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="822a5-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="822a5-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="822a5-128">Schema Name</span></span>  <br/> |<span data-ttu-id="822a5-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="822a5-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="822a5-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="822a5-130">Validation File</span></span>  <br/> |<span data-ttu-id="822a5-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="822a5-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="822a5-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="822a5-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="822a5-133">False</span><span class="sxs-lookup"><span data-stu-id="822a5-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="822a5-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="822a5-134">See also</span></span>



- [<span data-ttu-id="822a5-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="822a5-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

