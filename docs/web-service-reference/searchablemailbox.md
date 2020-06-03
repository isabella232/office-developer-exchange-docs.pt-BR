---
title: SearchableMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 339005cd-a3b9-47dd-bc7b-a860b699625b
description: O elemento SearchableMailbox especifica uma caixa de correio retornada de uma solicitação GetSearchableMailboxes.
ms.openlocfilehash: f790d9a707f10f64a776b2fc35255c233ad854b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467449"
---
# <a name="searchablemailbox"></a><span data-ttu-id="eaa67-103">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="eaa67-103">SearchableMailbox</span></span>

<span data-ttu-id="eaa67-104">O elemento **SearchableMailbox** especifica uma caixa de correio retornada de uma solicitação **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="eaa67-104">The **SearchableMailbox** element specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span> 
  
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

 <span data-ttu-id="eaa67-105">**SearchableMailboxType**</span><span class="sxs-lookup"><span data-stu-id="eaa67-105">**SearchableMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eaa67-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="eaa67-106">Attributes and elements</span></span>

<span data-ttu-id="eaa67-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="eaa67-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eaa67-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="eaa67-108">Attributes</span></span>

<span data-ttu-id="eaa67-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eaa67-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eaa67-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="eaa67-110">Child elements</span></span>

<span data-ttu-id="eaa67-111">[GUID](guid-ex15websvcsotherref.md)  |  [PrimarySmtpAddress (cadeia de caracteres)](primarysmtpaddress-string.md)  |  [IsExternalMailbox](isexternalmailbox.md)  |  [ExternalEmailAddress](externalemailaddress.md)  |  [DisplayName (cadeia de caracteres)](displayname-string.md)  |  [Membro Ismembership](ismembershipgroup.md)  |  [Referenceid](referenceid.md)</span><span class="sxs-lookup"><span data-stu-id="eaa67-111">[Guid](guid-ex15websvcsotherref.md) | [PrimarySmtpAddress (string)](primarysmtpaddress-string.md) | [IsExternalMailbox](isexternalmailbox.md) | [ExternalEmailAddress](externalemailaddress.md) | [DisplayName (string)](displayname-string.md) | [IsMembershipGroup](ismembershipgroup.md) | [ReferenceId](referenceid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="eaa67-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="eaa67-112">Parent elements</span></span>

[<span data-ttu-id="eaa67-113">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="eaa67-113">SearchableMailboxes</span></span>](searchablemailboxes.md)
  
## <a name="remarks"></a><span data-ttu-id="eaa67-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="eaa67-114">Remarks</span></span>

<span data-ttu-id="eaa67-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="eaa67-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="eaa67-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="eaa67-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eaa67-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="eaa67-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eaa67-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="eaa67-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eaa67-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="eaa67-119">Schema name</span></span>  <br/> |<span data-ttu-id="eaa67-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="eaa67-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="eaa67-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="eaa67-121">Validation file</span></span>  <br/> |<span data-ttu-id="eaa67-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="eaa67-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eaa67-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="eaa67-123">Can be empty</span></span>  <br/> ||
   

