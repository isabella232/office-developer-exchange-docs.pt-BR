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
description: O elemento GroupSids representa uma coleção de identificadores de segurança do objeto do grupo de serviços de diretório do Active Directory.
ms.openlocfilehash: 40f36176fcaa3e2160237f269fb2dc3b12bf8af2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530061"
---
# <a name="groupsids"></a><span data-ttu-id="2611f-103">GroupSids</span><span class="sxs-lookup"><span data-stu-id="2611f-103">GroupSids</span></span>

<span data-ttu-id="2611f-104">O elemento **GroupSids** representa uma coleção de identificadores de segurança do objeto do grupo de serviços de diretório do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2611f-104">The **GroupSids** element represents a collection of Active Directory directory service group object security identifiers.</span></span> 
  
```xml
<GroupSids>
   <GroupIdentifier/>
</GroupSids>
```

 <span data-ttu-id="2611f-105">**NonEmptyArrayOfGroupIdentifiersType**</span><span class="sxs-lookup"><span data-stu-id="2611f-105">**NonEmptyArrayOfGroupIdentifiersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2611f-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2611f-106">Attributes and elements</span></span>

<span data-ttu-id="2611f-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2611f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2611f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2611f-108">Attributes</span></span>

<span data-ttu-id="2611f-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2611f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2611f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2611f-110">Child elements</span></span>

|<span data-ttu-id="2611f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2611f-111">**Element**</span></span>|<span data-ttu-id="2611f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2611f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2611f-113">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="2611f-113">GroupIdentifier</span></span>](groupidentifier.md) <br/> |<span data-ttu-id="2611f-114">Representa um único identificador de segurança e atributo para um grupo de objetos do Active Directory do qual a conta é membro.</span><span class="sxs-lookup"><span data-stu-id="2611f-114">Represents a single security identifier and attribute for an Active Directory object group of which the account is a member.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2611f-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2611f-115">Parent elements</span></span>

|<span data-ttu-id="2611f-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2611f-116">**Element**</span></span>|<span data-ttu-id="2611f-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2611f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2611f-118">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="2611f-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="2611f-119">Usado no cabeçalho SOAP (Simple Object Access Protocol) para serialização de token na autenticação de servidor para servidor.</span><span class="sxs-lookup"><span data-stu-id="2611f-119">Used in the Simple Object Access Protocol (SOAP) header for token serialization in server-to-server authentication.</span></span> <span data-ttu-id="2611f-120">Não há suporte para serialização de token.</span><span class="sxs-lookup"><span data-stu-id="2611f-120">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2611f-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="2611f-121">Remarks</span></span>

<span data-ttu-id="2611f-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="2611f-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2611f-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2611f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2611f-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="2611f-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2611f-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2611f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2611f-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="2611f-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="2611f-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2611f-127">Validation File</span></span>  <br/> |<span data-ttu-id="2611f-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2611f-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2611f-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2611f-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="2611f-130">False</span><span class="sxs-lookup"><span data-stu-id="2611f-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2611f-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="2611f-131">See also</span></span>



- [<span data-ttu-id="2611f-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2611f-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

