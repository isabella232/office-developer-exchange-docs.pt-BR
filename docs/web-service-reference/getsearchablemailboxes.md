---
title: GetSearchableMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 949871f7-0d10-498e-84aa-f0652f1193be
description: O elemento GetSearchableMailboxes contém uma solicitação para obter uma lista de caixas de correio que o cliente tem permissão para executar uma pesquisa de descoberta eletrônica.
ms.openlocfilehash: 8cce18bb62d3840cb9883d20a380cc4f2193303e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752616"
---
# <a name="getsearchablemailboxes"></a><span data-ttu-id="26828-103">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="26828-103">GetSearchableMailboxes</span></span>

<span data-ttu-id="26828-104">O elemento **GetSearchableMailboxes** contém uma solicitação para obter uma lista de caixas de correio que o cliente tem permissão para executar uma pesquisa de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="26828-104">The **GetSearchableMailboxes** element contains a request to get a list of mailboxes that the client has permission to perform an eDiscovery search.</span></span> 
  
```XML
<GetSearchableMailboxes>
   <SearchFilter/>
   <ExpandGroupMembership/>
</GetSearchableMailboxes>
```

 <span data-ttu-id="26828-105">**GetSearchableMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="26828-105">**GetSearchableMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26828-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="26828-106">Attributes and elements</span></span>

<span data-ttu-id="26828-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="26828-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26828-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="26828-108">Attributes</span></span>

<span data-ttu-id="26828-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="26828-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26828-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="26828-110">Child elements</span></span>

<span data-ttu-id="26828-111">[SearchFilter](searchfilter.md) | [ExpandGroupMembership](expandgroupmembership.md)</span><span class="sxs-lookup"><span data-stu-id="26828-111">[SearchFilter](searchfilter.md) | [ExpandGroupMembership](expandgroupmembership.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="26828-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="26828-112">Parent elements</span></span>

<span data-ttu-id="26828-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="26828-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="26828-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="26828-114">Remarks</span></span>

<span data-ttu-id="26828-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="26828-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="26828-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="26828-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26828-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="26828-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26828-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="26828-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="26828-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="26828-119">Schema name</span></span>  <br/> |<span data-ttu-id="26828-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="26828-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="26828-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="26828-121">Validation file</span></span>  <br/> |<span data-ttu-id="26828-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="26828-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="26828-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="26828-123">Can be empty</span></span>  <br/> ||
   

