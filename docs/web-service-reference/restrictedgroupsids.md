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
description: O elemento RestrictedGroupSids representa uma coleção de grupos restritos do token de um usuário.
ms.openlocfilehash: 739a73d2ac4bdbbee03650d035271b5c8d9ea25a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465356"
---
# <a name="restrictedgroupsids"></a><span data-ttu-id="a6158-103">RestrictedGroupSids</span><span class="sxs-lookup"><span data-stu-id="a6158-103">RestrictedGroupSids</span></span>

<span data-ttu-id="a6158-104">O elemento **RestrictedGroupSids** representa uma coleção de grupos restritos do token de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a6158-104">The **RestrictedGroupSids** element represents a collection of restricted groups from a user's token.</span></span> 
  
```xml
<RestrictedGroupSids>
   <RestrictedGroupIdentifier/>
</RestrictedGroupSids>
```

 <span data-ttu-id="a6158-105">**NonEmptyArrayOfRestrictedGroupIdentifiersType**</span><span class="sxs-lookup"><span data-stu-id="a6158-105">**NonEmptyArrayOfRestrictedGroupIdentifiersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a6158-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a6158-106">Attributes and elements</span></span>

<span data-ttu-id="a6158-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a6158-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a6158-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a6158-108">Attributes</span></span>

<span data-ttu-id="a6158-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a6158-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a6158-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a6158-110">Child elements</span></span>

|<span data-ttu-id="a6158-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a6158-111">**Element**</span></span>|<span data-ttu-id="a6158-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a6158-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a6158-113">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="a6158-113">RestrictedGroupIdentifier</span></span>](restrictedgroupidentifier.md) <br/> |<span data-ttu-id="a6158-114">Representa o identificador de segurança do grupo (SID) e os atributos de um grupo restrito.</span><span class="sxs-lookup"><span data-stu-id="a6158-114">Represents the group security identifier (SID) and attributes for a restricted group.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a6158-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a6158-115">Parent elements</span></span>

|<span data-ttu-id="a6158-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a6158-116">**Element**</span></span>|<span data-ttu-id="a6158-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a6158-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a6158-118">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="a6158-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="a6158-119">Usado no cabeçalho SOAP para serialização de token na autenticação de servidor para servidor.</span><span class="sxs-lookup"><span data-stu-id="a6158-119">Used in the SOAP header for token serialization in server- to-server authentication.</span></span> <span data-ttu-id="a6158-120">Não há suporte para serialização de token.</span><span class="sxs-lookup"><span data-stu-id="a6158-120">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a6158-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="a6158-121">Remarks</span></span>

<span data-ttu-id="a6158-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="a6158-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a6158-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a6158-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a6158-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="a6158-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a6158-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a6158-125">Schema Name</span></span>  <br/> |<span data-ttu-id="a6158-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a6158-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="a6158-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a6158-127">Validation File</span></span>  <br/> |<span data-ttu-id="a6158-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a6158-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a6158-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a6158-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="a6158-130">False</span><span class="sxs-lookup"><span data-stu-id="a6158-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a6158-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="a6158-131">See also</span></span>



- [<span data-ttu-id="a6158-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a6158-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

