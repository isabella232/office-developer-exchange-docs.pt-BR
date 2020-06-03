---
title: MailboxMoveEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 73d09137-d3bd-46b3-954a-a358ead07c91
description: O elemento MailBoxMoveEnabled representa o sinalizador MailboxMoveEnabled (). O elemento MailBoxMoveEnabled é somente para uso interno. Esse elemento não é usado por clientes.
ms.openlocfilehash: 4072d1c231e7cf109a39445fc44fbbb624f6f3a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530737"
---
# <a name="mailboxmoveenabled-soap"></a><span data-ttu-id="d2e01-105">MailboxMoveEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d2e01-105">MailboxMoveEnabled (SOAP)</span></span>

<span data-ttu-id="d2e01-106">O elemento **MailBoxMoveEnabled** representa o sinalizador **MailBoxMoveEnabled ()** .</span><span class="sxs-lookup"><span data-stu-id="d2e01-106">The **MailBoxMoveEnabled** element represents the **MailboxMoveEnabled()** flag.</span></span> <span data-ttu-id="d2e01-107">O elemento **MailBoxMoveEnabled** é somente para uso interno.</span><span class="sxs-lookup"><span data-stu-id="d2e01-107">The **MailBoxMoveEnabled** element is for internal use only.</span></span> <span data-ttu-id="d2e01-108">Esse elemento não é usado por clientes.</span><span class="sxs-lookup"><span data-stu-id="d2e01-108">This element is not used by clients.</span></span> 
  
```XML
<MailBoxMoveEnabled>true | false</MailBoxMoveEnabled>
```

<span data-ttu-id="d2e01-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d2e01-109">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d2e01-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d2e01-110">Attributes and elements</span></span>

<span data-ttu-id="d2e01-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d2e01-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2e01-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="d2e01-112">Attributes</span></span>

<span data-ttu-id="d2e01-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2e01-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2e01-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d2e01-114">Child elements</span></span>

<span data-ttu-id="d2e01-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d2e01-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d2e01-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d2e01-116">Parent elements</span></span>

|<span data-ttu-id="d2e01-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d2e01-117">**Element**</span></span>|<span data-ttu-id="d2e01-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d2e01-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2e01-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d2e01-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="d2e01-120">Representa uma lista de relações de organização para uma única organização.</span><span class="sxs-lookup"><span data-stu-id="d2e01-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="d2e01-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d2e01-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2e01-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="d2e01-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d2e01-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d2e01-123">Schema Name</span></span>  <br/> |<span data-ttu-id="d2e01-124">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="d2e01-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d2e01-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d2e01-125">Validation File</span></span>  <br/> |<span data-ttu-id="d2e01-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d2e01-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d2e01-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d2e01-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="d2e01-128">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="d2e01-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d2e01-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="d2e01-129">See also</span></span>

- [<span data-ttu-id="d2e01-130">Operação GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d2e01-130">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

