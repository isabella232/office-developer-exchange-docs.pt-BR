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
description: O elemento SecurityIdentifier representa um formulário de segurança descritor definition language (SDDL) de um identificador de segurança (SID).
ms.openlocfilehash: c18d7d4505c618792497c32c7499eab9ac82989e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825314"
---
# <a name="securityidentifier"></a><span data-ttu-id="87c71-103">SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="87c71-103">SecurityIdentifier</span></span>

<span data-ttu-id="87c71-104">O elemento **SecurityIdentifier** representa um formulário de segurança descritor definition language (SDDL) de um identificador de segurança ( [SID](sid.md)).</span><span class="sxs-lookup"><span data-stu-id="87c71-104">The **SecurityIdentifier** element represents the security descriptor definition language (SDDL) form of a security identifier ( [SID](sid.md)).</span></span>
  
```xml
<SecurityIdentifier/>
```

 <span data-ttu-id="87c71-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="87c71-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="87c71-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="87c71-106">Attributes and elements</span></span>

<span data-ttu-id="87c71-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="87c71-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="87c71-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="87c71-108">Attributes</span></span>

<span data-ttu-id="87c71-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="87c71-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="87c71-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="87c71-110">Child elements</span></span>

<span data-ttu-id="87c71-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="87c71-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="87c71-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="87c71-112">Parent elements</span></span>

|<span data-ttu-id="87c71-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="87c71-113">**Element**</span></span>|<span data-ttu-id="87c71-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="87c71-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87c71-115">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="87c71-115">GroupIdentifier</span></span>](groupidentifier.md) <br/> |<span data-ttu-id="87c71-116">Representa um identificador de segurança único e o atributo para um grupo de objetos do Active Directory do qual a conta é membro.</span><span class="sxs-lookup"><span data-stu-id="87c71-116">Represents a single security identifier and attribute for an Active Directory object group of which the account is a member.</span></span>  <br/> <span data-ttu-id="87c71-117">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="87c71-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SerializedSecurityContext/GroupSids/GroupIdentifier[i]` <br/> |
|[<span data-ttu-id="87c71-118">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="87c71-118">RestrictedGroupIdentifier</span></span>](restrictedgroupidentifier.md) <br/> |<span data-ttu-id="87c71-119">Representa o identificador de segurança de grupo e os atributos de um grupo restrito dentro de um token de usuário.</span><span class="sxs-lookup"><span data-stu-id="87c71-119">Represents the group security identifier and attributes for a restricted group within a user token.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="87c71-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="87c71-120">Remarks</span></span>

<span data-ttu-id="87c71-121">Este elemento é usado no cabeçalho simples (SOAP Object Access Protocol).</span><span class="sxs-lookup"><span data-stu-id="87c71-121">This element is used in the Simple Object Access Protocol (SOAP) header.</span></span>
  
<span data-ttu-id="87c71-122">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="87c71-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="87c71-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="87c71-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="87c71-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="87c71-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="87c71-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="87c71-125">Schema Name</span></span>  <br/> |<span data-ttu-id="87c71-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="87c71-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="87c71-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="87c71-127">Validation File</span></span>  <br/> |<span data-ttu-id="87c71-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="87c71-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="87c71-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="87c71-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="87c71-130">False</span><span class="sxs-lookup"><span data-stu-id="87c71-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="87c71-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="87c71-131">See also</span></span>



- [<span data-ttu-id="87c71-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="87c71-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

