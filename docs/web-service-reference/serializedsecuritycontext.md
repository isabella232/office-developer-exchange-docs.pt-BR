---
title: SerializedSecurityContext
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SerializedSecurityContext
api_type:
- schema
ms.assetid: a02c4fc1-ed1a-40d9-a18e-6cfdae21a690
description: O elemento SerializedSecurityContext é usado no cabeçalho simples (SOAP Object Access Protocol) para serialização de token de autenticação de servidor-para-servidor. Serialização de token não é suportada.
ms.openlocfilehash: c5590551dc0780d918b05902e4f48fb9d1390b59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825363"
---
# <a name="serializedsecuritycontext"></a><span data-ttu-id="728f3-104">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="728f3-104">SerializedSecurityContext</span></span>

<span data-ttu-id="728f3-105">O elemento **SerializedSecurityContext** é usado no cabeçalho simples (SOAP Object Access Protocol) para serialização de token de autenticação de servidor-para-servidor.</span><span class="sxs-lookup"><span data-stu-id="728f3-105">The **SerializedSecurityContext** element is used in the Simple Object Access Protocol (SOAP) header for token serialization in server-to-server authentication.</span></span> <span data-ttu-id="728f3-106">Serialização de token não é suportada.</span><span class="sxs-lookup"><span data-stu-id="728f3-106">Token serialization is not supported.</span></span> 
  
```xml
<SerializedSecurityContext>
   <UserSid/>
   <GroupSids/>
   <RestrictedGroupSids/>
   <PrimarySmtpAddress/>
</SerializedSecurityContext>
```

 <span data-ttu-id="728f3-107">**SerializedSecurityContextType**</span><span class="sxs-lookup"><span data-stu-id="728f3-107">**SerializedSecurityContextType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="728f3-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="728f3-108">Attributes and elements</span></span>

<span data-ttu-id="728f3-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="728f3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="728f3-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="728f3-110">Attributes</span></span>

<span data-ttu-id="728f3-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="728f3-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="728f3-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="728f3-112">Child elements</span></span>

|<span data-ttu-id="728f3-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="728f3-113">**Element**</span></span>|<span data-ttu-id="728f3-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="728f3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="728f3-115">UserSid</span><span class="sxs-lookup"><span data-stu-id="728f3-115">UserSid</span></span>](usersid.md) <br/> |<span data-ttu-id="728f3-116">Representa o formato segurança descritor definition language (SDDL) o identificador de segurança do usuário em um cabeçalho SOAP de contexto de segurança serializados.</span><span class="sxs-lookup"><span data-stu-id="728f3-116">Represents the security descriptor definition language (SDDL) form of the user security identifier in a serialized security context SOAP header.</span></span>  <br/> |
|[<span data-ttu-id="728f3-117">GroupSids</span><span class="sxs-lookup"><span data-stu-id="728f3-117">GroupSids</span></span>](groupsids.md) <br/> |<span data-ttu-id="728f3-118">Representa uma coleção de identificadores de segurança do objeto de grupo do Active Directory directory service.</span><span class="sxs-lookup"><span data-stu-id="728f3-118">Represents a collection of Active Directory directory service group object security identifiers.</span></span>  <br/> |
|[<span data-ttu-id="728f3-119">RestrictedGroupSids</span><span class="sxs-lookup"><span data-stu-id="728f3-119">RestrictedGroupSids</span></span>](restrictedgroupsids.md) <br/> |<span data-ttu-id="728f3-120">Representa o identificador de segurança de grupo e os atributos de um grupo restrito.</span><span class="sxs-lookup"><span data-stu-id="728f3-120">Represents the group security identifier and attributes for a restricted group.</span></span>  <br/> |
|[<span data-ttu-id="728f3-121">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="728f3-121">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="728f3-122">Representa o endereço de Simple Mail Transfer Protocol (SMTP) principal de uma conta que serão usados para autorização de servidor-para-servidor.</span><span class="sxs-lookup"><span data-stu-id="728f3-122">Represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for server-to-server authorization.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="728f3-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="728f3-123">Parent elements</span></span>

<span data-ttu-id="728f3-124">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="728f3-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="728f3-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="728f3-125">Remarks</span></span>

<span data-ttu-id="728f3-126">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor (CAS) de acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="728f3-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server (CAS) role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="728f3-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="728f3-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="728f3-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="728f3-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="728f3-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="728f3-129">Schema Name</span></span>  <br/> |<span data-ttu-id="728f3-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="728f3-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="728f3-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="728f3-131">Validation File</span></span>  <br/> |<span data-ttu-id="728f3-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="728f3-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="728f3-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="728f3-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="728f3-134">False</span><span class="sxs-lookup"><span data-stu-id="728f3-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="728f3-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="728f3-135">See also</span></span>



- [<span data-ttu-id="728f3-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="728f3-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="728f3-137">Autorização de servidor-para-servidor no EWS</span><span class="sxs-lookup"><span data-stu-id="728f3-137">Server-to-server authorization in EWS</span></span>](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

