---
title: SearchableMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 339005cd-a3b9-47dd-bc7b-a860b699625b
description: O elemento SearchableMailbox Especifica uma caixa de correio retornados de uma solicitação de GetSearchableMailboxes.
ms.openlocfilehash: 0d0981d050fa388e83eaa8408b60d305296c1f36
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825284"
---
# <a name="searchablemailbox"></a><span data-ttu-id="4768d-103">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="4768d-103">SearchableMailbox</span></span>

<span data-ttu-id="4768d-104">O elemento **SearchableMailbox** Especifica uma caixa de correio retornados de uma solicitação de **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="4768d-104">The **SearchableMailbox** element specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<SearchableMailbox>
   <Guid/>
   <PrimarySmtpAddress/>
   <IsExternalMailbox/>
   <ExternalEmailAddress/>
   <DisplayName/>
   <IsMembershipGroup/>
   <ReferenceId/>
</SearchableMailbox>
```

 <span data-ttu-id="4768d-105">**SearchableMailboxType**</span><span class="sxs-lookup"><span data-stu-id="4768d-105">**SearchableMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4768d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4768d-106">Attributes and elements</span></span>

<span data-ttu-id="4768d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4768d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4768d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4768d-108">Attributes</span></span>

<span data-ttu-id="4768d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4768d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4768d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4768d-110">Child elements</span></span>

<span data-ttu-id="4768d-111">[GUID](guid-ex15websvcsotherref.md) | [PrimarySmtpAddress (string)](primarysmtpaddress-string.md) | [IsExternalMailbox](isexternalmailbox.md) | [ExternalEmailAddress](externalemailaddress.md) | [DisplayName (string)](displayname-string.md) | [IsMembershipGroup](ismembershipgroup.md)  |  [ ID de referência](referenceid.md)</span><span class="sxs-lookup"><span data-stu-id="4768d-111">[Guid](guid-ex15websvcsotherref.md) | [PrimarySmtpAddress (string)](primarysmtpaddress-string.md) | [IsExternalMailbox](isexternalmailbox.md) | [ExternalEmailAddress](externalemailaddress.md) | [DisplayName (string)](displayname-string.md) | [IsMembershipGroup](ismembershipgroup.md) | [ReferenceId](referenceid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4768d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4768d-112">Parent elements</span></span>

[<span data-ttu-id="4768d-113">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="4768d-113">SearchableMailboxes</span></span>](searchablemailboxes.md)
  
## <a name="remarks"></a><span data-ttu-id="4768d-114">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="4768d-114">Remarks</span></span>

<span data-ttu-id="4768d-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4768d-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4768d-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4768d-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4768d-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4768d-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4768d-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="4768d-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4768d-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4768d-119">Schema name</span></span>  <br/> |<span data-ttu-id="4768d-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4768d-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="4768d-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4768d-121">Validation file</span></span>  <br/> |<span data-ttu-id="4768d-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4768d-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4768d-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="4768d-123">Can be empty</span></span>  <br/> ||
   

