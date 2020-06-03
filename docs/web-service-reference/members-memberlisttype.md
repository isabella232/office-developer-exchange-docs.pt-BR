---
title: Membros (MemberListType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Members
api_type:
- schema
ms.assetid: cbd38049-2ef7-40bf-9bec-0469af0f58ec
description: O elemento Members fornece a lista de membros para uma lista de distribuição.
ms.openlocfilehash: 2cdfb81dfbc223db365d49ed44d4893339eb4653
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462427"
---
# <a name="members-memberlisttype"></a><span data-ttu-id="922e4-103">Membros (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="922e4-103">Members (MemberListType)</span></span>

<span data-ttu-id="922e4-104">O elemento **Members** fornece a lista de membros para uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="922e4-104">The **Members** element provides the list of members for a distribution list.</span></span> 
  
```xml
<Members>
   <Member/>
</Members>
```

<span data-ttu-id="922e4-105">**MemberListType**</span><span class="sxs-lookup"><span data-stu-id="922e4-105">**MemberListType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="922e4-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="922e4-106">Attributes and elements</span></span>

<span data-ttu-id="922e4-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="922e4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="922e4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="922e4-108">Attributes</span></span>

<span data-ttu-id="922e4-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="922e4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="922e4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="922e4-110">Child elements</span></span>

|<span data-ttu-id="922e4-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="922e4-111">**Element**</span></span>|<span data-ttu-id="922e4-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="922e4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="922e4-113">Membro</span><span class="sxs-lookup"><span data-stu-id="922e4-113">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="922e4-114">Fornece um identificador para um endereço de email totalmente resolvido e o status desse endereço no servidor.</span><span class="sxs-lookup"><span data-stu-id="922e4-114">Provides an identifier for a fully resolved e-mail address, and the status of that address on the server.</span></span> <span data-ttu-id="922e4-115">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="922e4-115">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="922e4-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="922e4-116">Parent elements</span></span>

|<span data-ttu-id="922e4-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="922e4-117">**Element**</span></span>|<span data-ttu-id="922e4-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="922e4-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="922e4-119">DistributionList</span><span class="sxs-lookup"><span data-stu-id="922e4-119">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="922e4-120">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="922e4-120">Represents a distribution list.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="922e4-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="922e4-121">Remarks</span></span>

<span data-ttu-id="922e4-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="922e4-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="922e4-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="922e4-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="922e4-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="922e4-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="922e4-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="922e4-125">Schema Name</span></span>  <br/> |<span data-ttu-id="922e4-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="922e4-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="922e4-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="922e4-127">Validation File</span></span>  <br/> |<span data-ttu-id="922e4-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="922e4-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="922e4-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="922e4-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="922e4-130">False</span><span class="sxs-lookup"><span data-stu-id="922e4-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="922e4-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="922e4-131">See also</span></span>

- [<span data-ttu-id="922e4-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="922e4-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

