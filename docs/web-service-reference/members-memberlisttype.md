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
description: O elemento de membros fornece a lista de membros para uma lista de distribuição.
ms.openlocfilehash: 8cf9ed7a64a908614ce7be30a9bef631739fcebf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824439"
---
# <a name="members-memberlisttype"></a><span data-ttu-id="9b221-103">Membros (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="9b221-103">Members (MemberListType)</span></span>

<span data-ttu-id="9b221-104">O elemento de **membros** fornece a lista de membros para uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="9b221-104">The **Members** element provides the list of members for a distribution list.</span></span> 
  
```xml
<Members>
   <Member/>
</Members>
```

<span data-ttu-id="9b221-105">**MemberListType**</span><span class="sxs-lookup"><span data-stu-id="9b221-105">**MemberListType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9b221-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9b221-106">Attributes and elements</span></span>

<span data-ttu-id="9b221-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9b221-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b221-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9b221-108">Attributes</span></span>

<span data-ttu-id="9b221-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9b221-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b221-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9b221-110">Child elements</span></span>

|<span data-ttu-id="9b221-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9b221-111">**Element**</span></span>|<span data-ttu-id="9b221-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9b221-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b221-113">Membro</span><span class="sxs-lookup"><span data-stu-id="9b221-113">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9b221-114">Fornece um identificador para um endereço de email totalmente resolvido e o status de endereço no servidor.</span><span class="sxs-lookup"><span data-stu-id="9b221-114">Provides an identifier for a fully resolved e-mail address, and the status of that address on the server.</span></span> <span data-ttu-id="9b221-115">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="9b221-115">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9b221-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9b221-116">Parent elements</span></span>

|<span data-ttu-id="9b221-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9b221-117">**Element**</span></span>|<span data-ttu-id="9b221-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9b221-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b221-119">DistributionList</span><span class="sxs-lookup"><span data-stu-id="9b221-119">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="9b221-120">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="9b221-120">Represents a distribution list.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9b221-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="9b221-121">Remarks</span></span>

<span data-ttu-id="9b221-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b221-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b221-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9b221-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b221-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="9b221-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9b221-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9b221-125">Schema Name</span></span>  <br/> |<span data-ttu-id="9b221-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9b221-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="9b221-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9b221-127">Validation File</span></span>  <br/> |<span data-ttu-id="9b221-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9b221-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9b221-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9b221-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="9b221-130">False</span><span class="sxs-lookup"><span data-stu-id="9b221-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9b221-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="9b221-131">See also</span></span>

- [<span data-ttu-id="9b221-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9b221-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

