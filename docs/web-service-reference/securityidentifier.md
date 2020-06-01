---
title: SecurityIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SecurityIdentifier
api_type:
- schema
ms.assetid: f7656729-f2c9-41cc-b1ec-60f480fc4dab
description: O elemento SecurityIdentifier representa a forma SDDL (Security Descriptor Definition Language) de um identificador de segurança (SID).
ms.openlocfilehash: c55e4a7f7f0b8f8a40e6fcaf8d18e253a6da2679
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468800"
---
# <a name="securityidentifier"></a><span data-ttu-id="58051-103">SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="58051-103">SecurityIdentifier</span></span>

<span data-ttu-id="58051-104">O elemento **SecurityIdentifier** representa a forma SDDL (Security Descriptor Definition Language) de um identificador de segurança ( [Sid](sid.md)).</span><span class="sxs-lookup"><span data-stu-id="58051-104">The **SecurityIdentifier** element represents the security descriptor definition language (SDDL) form of a security identifier ( [SID](sid.md)).</span></span>
  
```xml
<SecurityIdentifier/>
```

 <span data-ttu-id="58051-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="58051-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="58051-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="58051-106">Attributes and elements</span></span>

<span data-ttu-id="58051-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="58051-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="58051-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="58051-108">Attributes</span></span>

<span data-ttu-id="58051-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58051-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="58051-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="58051-110">Child elements</span></span>

<span data-ttu-id="58051-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="58051-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="58051-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="58051-112">Parent elements</span></span>

|<span data-ttu-id="58051-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="58051-113">**Element**</span></span>|<span data-ttu-id="58051-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="58051-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58051-115">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="58051-115">GroupIdentifier</span></span>](groupidentifier.md) <br/> |<span data-ttu-id="58051-116">Representa um único identificador de segurança e atributo para um grupo de objetos do Active Directory do qual a conta é membro.</span><span class="sxs-lookup"><span data-stu-id="58051-116">Represents a single security identifier and attribute for an Active Directory object group of which the account is a member.</span></span>  <br/> <span data-ttu-id="58051-117">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="58051-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SerializedSecurityContext/GroupSids/GroupIdentifier[i]` <br/> |
|[<span data-ttu-id="58051-118">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="58051-118">RestrictedGroupIdentifier</span></span>](restrictedgroupidentifier.md) <br/> |<span data-ttu-id="58051-119">Representa o identificador de segurança do grupo e os atributos de um grupo restrito dentro de um token de usuário.</span><span class="sxs-lookup"><span data-stu-id="58051-119">Represents the group security identifier and attributes for a restricted group within a user token.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="58051-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="58051-120">Remarks</span></span>

<span data-ttu-id="58051-121">Este elemento é usado no cabeçalho SOAP (Simple Object Access Protocol).</span><span class="sxs-lookup"><span data-stu-id="58051-121">This element is used in the Simple Object Access Protocol (SOAP) header.</span></span>
  
<span data-ttu-id="58051-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="58051-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="58051-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="58051-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="58051-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="58051-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="58051-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="58051-125">Schema Name</span></span>  <br/> |<span data-ttu-id="58051-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="58051-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="58051-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="58051-127">Validation File</span></span>  <br/> |<span data-ttu-id="58051-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="58051-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="58051-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="58051-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="58051-130">False</span><span class="sxs-lookup"><span data-stu-id="58051-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="58051-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="58051-131">See also</span></span>



- [<span data-ttu-id="58051-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="58051-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

