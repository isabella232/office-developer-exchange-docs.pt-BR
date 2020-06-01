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
description: O elemento SerializedSecurityContext é usado no cabeçalho SOAP (Simple Object Access Protocol) para serialização de token em autenticação de servidor para servidor. Não há suporte para serialização de token.
ms.openlocfilehash: 58fea1c7f613315d59e81935561f92f318afc769
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462049"
---
# <a name="serializedsecuritycontext"></a><span data-ttu-id="8a75e-104">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="8a75e-104">SerializedSecurityContext</span></span>

<span data-ttu-id="8a75e-105">O elemento **SerializedSecurityContext** é usado no cabeçalho SOAP (Simple Object Access Protocol) para serialização de token em autenticação de servidor para servidor.</span><span class="sxs-lookup"><span data-stu-id="8a75e-105">The **SerializedSecurityContext** element is used in the Simple Object Access Protocol (SOAP) header for token serialization in server-to-server authentication.</span></span> <span data-ttu-id="8a75e-106">Não há suporte para serialização de token.</span><span class="sxs-lookup"><span data-stu-id="8a75e-106">Token serialization is not supported.</span></span> 
  
```xml
<SerializedSecurityContext>
   <UserSid/>
   <GroupSids/>
   <RestrictedGroupSids/>
   <PrimarySmtpAddress/>
</SerializedSecurityContext>
```

 <span data-ttu-id="8a75e-107">**SerializedSecurityContextType**</span><span class="sxs-lookup"><span data-stu-id="8a75e-107">**SerializedSecurityContextType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8a75e-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8a75e-108">Attributes and elements</span></span>

<span data-ttu-id="8a75e-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8a75e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8a75e-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="8a75e-110">Attributes</span></span>

<span data-ttu-id="8a75e-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8a75e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8a75e-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8a75e-112">Child elements</span></span>

|<span data-ttu-id="8a75e-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8a75e-113">**Element**</span></span>|<span data-ttu-id="8a75e-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8a75e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a75e-115">Userid</span><span class="sxs-lookup"><span data-stu-id="8a75e-115">UserSid</span></span>](usersid.md) <br/> |<span data-ttu-id="8a75e-116">Representa a forma SDDL (Security Descriptor Definition Language) do identificador de segurança do usuário em um cabeçalho SOAP de contexto de segurança serializado.</span><span class="sxs-lookup"><span data-stu-id="8a75e-116">Represents the security descriptor definition language (SDDL) form of the user security identifier in a serialized security context SOAP header.</span></span>  <br/> |
|[<span data-ttu-id="8a75e-117">GroupSids</span><span class="sxs-lookup"><span data-stu-id="8a75e-117">GroupSids</span></span>](groupsids.md) <br/> |<span data-ttu-id="8a75e-118">Representa uma coleção de identificadores de segurança do objeto do grupo de serviços de diretório do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8a75e-118">Represents a collection of Active Directory directory service group object security identifiers.</span></span>  <br/> |
|[<span data-ttu-id="8a75e-119">RestrictedGroupSids</span><span class="sxs-lookup"><span data-stu-id="8a75e-119">RestrictedGroupSids</span></span>](restrictedgroupsids.md) <br/> |<span data-ttu-id="8a75e-120">Representa o identificador de segurança do grupo e os atributos de um grupo restrito.</span><span class="sxs-lookup"><span data-stu-id="8a75e-120">Represents the group security identifier and attributes for a restricted group.</span></span>  <br/> |
|[<span data-ttu-id="8a75e-121">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="8a75e-121">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="8a75e-122">Representa o endereço SMTP (Simple Mail Transfer Protocol) principal de uma conta a ser usada para a autorização de servidor para servidor.</span><span class="sxs-lookup"><span data-stu-id="8a75e-122">Represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for server-to-server authorization.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8a75e-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8a75e-123">Parent elements</span></span>

<span data-ttu-id="8a75e-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8a75e-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8a75e-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="8a75e-125">Remarks</span></span>

<span data-ttu-id="8a75e-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para cliente (CAS) instalada.</span><span class="sxs-lookup"><span data-stu-id="8a75e-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server (CAS) role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8a75e-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8a75e-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8a75e-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="8a75e-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8a75e-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8a75e-129">Schema Name</span></span>  <br/> |<span data-ttu-id="8a75e-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8a75e-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="8a75e-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8a75e-131">Validation File</span></span>  <br/> |<span data-ttu-id="8a75e-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8a75e-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8a75e-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8a75e-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="8a75e-134">False</span><span class="sxs-lookup"><span data-stu-id="8a75e-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8a75e-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="8a75e-135">See also</span></span>



- [<span data-ttu-id="8a75e-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8a75e-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="8a75e-137">Autorização de servidor para servidor no EWS</span><span class="sxs-lookup"><span data-stu-id="8a75e-137">Server-to-server authorization in EWS</span></span>](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

