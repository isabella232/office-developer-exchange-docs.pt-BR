---
title: GroupSids
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupSids
api_type:
- schema
ms.assetid: ebb00653-83f0-4080-a902-c38df6719800
description: O elemento GroupSids representa uma coleção de identificadores de segurança do objeto de grupo do Active Directory directory service.
ms.openlocfilehash: c24c8ea3c3b7d37f41986997ed924c951b4a48ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823790"
---
# <a name="groupsids"></a><span data-ttu-id="a7c8d-103">GroupSids</span><span class="sxs-lookup"><span data-stu-id="a7c8d-103">GroupSids</span></span>

<span data-ttu-id="a7c8d-104">O elemento **GroupSids** representa uma coleção de identificadores de segurança do objeto de grupo do Active Directory directory service.</span><span class="sxs-lookup"><span data-stu-id="a7c8d-104">The **GroupSids** element represents a collection of Active Directory directory service group object security identifiers.</span></span> 
  
```xml
<GroupSids>
   <GroupIdentifier/>
</GroupSids>
```

 <span data-ttu-id="a7c8d-105">**NonEmptyArrayOfGroupIdentifiersType**</span><span class="sxs-lookup"><span data-stu-id="a7c8d-105">**NonEmptyArrayOfGroupIdentifiersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a7c8d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a7c8d-106">Attributes and elements</span></span>

<span data-ttu-id="a7c8d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a7c8d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a7c8d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a7c8d-108">Attributes</span></span>

<span data-ttu-id="a7c8d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a7c8d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a7c8d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a7c8d-110">Child elements</span></span>

|<span data-ttu-id="a7c8d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a7c8d-111">**Element**</span></span>|<span data-ttu-id="a7c8d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a7c8d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7c8d-113">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="a7c8d-113">GroupIdentifier</span></span>](groupidentifier.md) <br/> |<span data-ttu-id="a7c8d-114">Representa um identificador de segurança único e o atributo para um grupo de objetos do Active Directory do qual a conta é membro.</span><span class="sxs-lookup"><span data-stu-id="a7c8d-114">Represents a single security identifier and attribute for an Active Directory object group of which the account is a member.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a7c8d-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a7c8d-115">Parent elements</span></span>

|<span data-ttu-id="a7c8d-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a7c8d-116">**Element**</span></span>|<span data-ttu-id="a7c8d-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a7c8d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7c8d-118">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="a7c8d-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="a7c8d-119">Usado no cabeçalho simples (SOAP Object Access Protocol) para serialização de token de autenticação de servidor-para-servidor.</span><span class="sxs-lookup"><span data-stu-id="a7c8d-119">Used in the Simple Object Access Protocol (SOAP) header for token serialization in server-to-server authentication.</span></span> <span data-ttu-id="a7c8d-120">Serialização de token não é suportada.</span><span class="sxs-lookup"><span data-stu-id="a7c8d-120">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a7c8d-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="a7c8d-121">Remarks</span></span>

<span data-ttu-id="a7c8d-122">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="a7c8d-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a7c8d-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a7c8d-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a7c8d-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="a7c8d-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a7c8d-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a7c8d-125">Schema Name</span></span>  <br/> |<span data-ttu-id="a7c8d-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a7c8d-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="a7c8d-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a7c8d-127">Validation File</span></span>  <br/> |<span data-ttu-id="a7c8d-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a7c8d-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a7c8d-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a7c8d-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="a7c8d-130">False</span><span class="sxs-lookup"><span data-stu-id="a7c8d-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a7c8d-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="a7c8d-131">See also</span></span>



- [<span data-ttu-id="a7c8d-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a7c8d-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

