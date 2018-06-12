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
description: O elemento RestrictGroupIdentifier representa o identificador de segurança (SID) do grupo e os atributos de um grupo restrito dentro de um token de usuário.
ms.openlocfilehash: c6db8672b2afa855e83f2e9a2bf84c9ff33bdc7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825206"
---
# <a name="restrictedgroupidentifier"></a><span data-ttu-id="40392-103">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="40392-103">RestrictedGroupIdentifier</span></span>

<span data-ttu-id="40392-104">O elemento **RestrictGroupIdentifier** representa o identificador de segurança (SID) do grupo e os atributos de um grupo restrito dentro de um token de usuário.</span><span class="sxs-lookup"><span data-stu-id="40392-104">The **RestrictGroupIdentifier** element represents the group security identifier (SID) and attributes for a restricted group within a user token.</span></span> 
  
```xml
<RestrictedGroupIdentifier Attributes="">
   <SecurityIdentifier/>
</RestrictedGroupIdentifier>
```

 <span data-ttu-id="40392-105">**SidAndAttributesType**</span><span class="sxs-lookup"><span data-stu-id="40392-105">**SidAndAttributesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="40392-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="40392-106">Attributes and elements</span></span>

<span data-ttu-id="40392-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="40392-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="40392-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="40392-108">Attributes</span></span>

|<span data-ttu-id="40392-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="40392-109">**Attribute**</span></span>|<span data-ttu-id="40392-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="40392-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="40392-111">**Attributes**</span><span class="sxs-lookup"><span data-stu-id="40392-111">**Attributes**</span></span> <br/> |<span data-ttu-id="40392-112">Contém atributos de grupo.</span><span class="sxs-lookup"><span data-stu-id="40392-112">Contains group attributes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="40392-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="40392-113">Child elements</span></span>

|<span data-ttu-id="40392-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="40392-114">**Element**</span></span>|<span data-ttu-id="40392-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="40392-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40392-116">SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="40392-116">SecurityIdentifier</span></span>](securityidentifier.md) <br/> |<span data-ttu-id="40392-117">Representa o formulário de segurança descritor definition language (SDDL) de um identificador de segurança.</span><span class="sxs-lookup"><span data-stu-id="40392-117">Represents the security descriptor definition language (SDDL) form of a security identifier.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="40392-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="40392-118">Parent elements</span></span>

|<span data-ttu-id="40392-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="40392-119">**Element**</span></span>|<span data-ttu-id="40392-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="40392-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40392-121">RestrictedGroupSids</span><span class="sxs-lookup"><span data-stu-id="40392-121">RestrictedGroupSids</span></span>](restrictedgroupsids.md) <br/> |<span data-ttu-id="40392-122">Representa uma coleção de grupos restritos dentro de um token de usuário.</span><span class="sxs-lookup"><span data-stu-id="40392-122">Represents a collection of restricted groups within a user token.</span></span> <span data-ttu-id="40392-123">Serialização de token não é suportada.</span><span class="sxs-lookup"><span data-stu-id="40392-123">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="40392-124">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="40392-124">Remarks</span></span>

<span data-ttu-id="40392-125">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="40392-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="40392-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="40392-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="40392-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="40392-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="40392-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="40392-128">Schema Name</span></span>  <br/> |<span data-ttu-id="40392-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="40392-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="40392-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="40392-130">Validation File</span></span>  <br/> |<span data-ttu-id="40392-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="40392-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="40392-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="40392-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="40392-133">False</span><span class="sxs-lookup"><span data-stu-id="40392-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="40392-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="40392-134">See also</span></span>



- [<span data-ttu-id="40392-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="40392-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

