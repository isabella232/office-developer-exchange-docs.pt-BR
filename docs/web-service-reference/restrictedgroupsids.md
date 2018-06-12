---
title: RestrictedGroupSids
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RestrictedGroupSids
api_type:
- schema
ms.assetid: 569ab552-5616-444a-a7f5-de366a684a34
description: O elemento RestrictedGroupSids representa uma coleção dos grupos restritos de um token do usuário.
ms.openlocfilehash: fcfee809261c7ed0a4e0d092c091841fec641e46
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825201"
---
# <a name="restrictedgroupsids"></a><span data-ttu-id="8816c-103">RestrictedGroupSids</span><span class="sxs-lookup"><span data-stu-id="8816c-103">RestrictedGroupSids</span></span>

<span data-ttu-id="8816c-104">O elemento **RestrictedGroupSids** representa uma coleção dos grupos restritos de um token do usuário.</span><span class="sxs-lookup"><span data-stu-id="8816c-104">The **RestrictedGroupSids** element represents a collection of restricted groups from a user's token.</span></span> 
  
```xml
<RestrictedGroupSids>
   <RestrictedGroupIdentifier/>
</RestrictedGroupSids>
```

 <span data-ttu-id="8816c-105">**NonEmptyArrayOfRestrictedGroupIdentifiersType**</span><span class="sxs-lookup"><span data-stu-id="8816c-105">**NonEmptyArrayOfRestrictedGroupIdentifiersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8816c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8816c-106">Attributes and elements</span></span>

<span data-ttu-id="8816c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8816c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8816c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8816c-108">Attributes</span></span>

<span data-ttu-id="8816c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8816c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8816c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8816c-110">Child elements</span></span>

|<span data-ttu-id="8816c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8816c-111">**Element**</span></span>|<span data-ttu-id="8816c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8816c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8816c-113">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="8816c-113">RestrictedGroupIdentifier</span></span>](restrictedgroupidentifier.md) <br/> |<span data-ttu-id="8816c-114">Representa o identificador de segurança (SID) do grupo e os atributos de um grupo restrito.</span><span class="sxs-lookup"><span data-stu-id="8816c-114">Represents the group security identifier (SID) and attributes for a restricted group.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8816c-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8816c-115">Parent elements</span></span>

|<span data-ttu-id="8816c-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8816c-116">**Element**</span></span>|<span data-ttu-id="8816c-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8816c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8816c-118">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="8816c-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="8816c-119">Usado no cabeçalho SOAP para serialização de token de autenticação de servidor-para-servidor.</span><span class="sxs-lookup"><span data-stu-id="8816c-119">Used in the SOAP header for token serialization in server- to-server authentication.</span></span> <span data-ttu-id="8816c-120">Serialização de token não é suportada.</span><span class="sxs-lookup"><span data-stu-id="8816c-120">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8816c-121">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="8816c-121">Remarks</span></span>

<span data-ttu-id="8816c-122">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="8816c-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8816c-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8816c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8816c-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="8816c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8816c-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8816c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="8816c-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8816c-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="8816c-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8816c-127">Validation File</span></span>  <br/> |<span data-ttu-id="8816c-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8816c-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8816c-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8816c-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="8816c-130">False</span><span class="sxs-lookup"><span data-stu-id="8816c-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8816c-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="8816c-131">See also</span></span>



- [<span data-ttu-id="8816c-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8816c-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

