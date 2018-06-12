---
title: SearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4a53989e-eca6-45c4-afac-4d6ac19597d2
description: O elemento SearchScope Especifica o escopo de uma pesquisa.
ms.openlocfilehash: 352292952c735e7d3893790a660096c6b6966536
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825315"
---
# <a name="searchscope"></a><span data-ttu-id="9d60f-103">SearchScope</span><span class="sxs-lookup"><span data-stu-id="9d60f-103">SearchScope</span></span>

<span data-ttu-id="9d60f-104">O elemento **SearchScope** Especifica o escopo de uma pesquisa.</span><span class="sxs-lookup"><span data-stu-id="9d60f-104">The **SearchScope** element specifies the scope of a search.</span></span> 
  
```XML
<SearchScope> PrimaryOnly | ArchiveOnly | All </SearchScope>
```

 <span data-ttu-id="9d60f-105">**MailboxSearchLocationType**</span><span class="sxs-lookup"><span data-stu-id="9d60f-105">**MailboxSearchLocationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d60f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9d60f-106">Attributes and elements</span></span>

<span data-ttu-id="9d60f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9d60f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d60f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9d60f-108">Attributes</span></span>

<span data-ttu-id="9d60f-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9d60f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d60f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9d60f-110">Child elements</span></span>

<span data-ttu-id="9d60f-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9d60f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9d60f-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9d60f-112">Parent elements</span></span>

[<span data-ttu-id="9d60f-113">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="9d60f-113">MailboxSearchScope</span></span>](mailboxsearchscope.md)
  
## <a name="text-value"></a><span data-ttu-id="9d60f-114">Text value</span><span class="sxs-lookup"><span data-stu-id="9d60f-114">Text value</span></span>

<span data-ttu-id="9d60f-115">O valor de texto do elemento **SearchScope** indica o tipo de caixa de correio que será pesquisado para uma pesquisa de descoberta.</span><span class="sxs-lookup"><span data-stu-id="9d60f-115">The text value of the **SearchScope** element indicates the mailbox type that is searched for a discovery search.</span></span> <span data-ttu-id="9d60f-116">Um valor de texto de **PrimaryOnly** indica que a caixa de correio principal é pesquisada.</span><span class="sxs-lookup"><span data-stu-id="9d60f-116">A text value of **PrimaryOnly** indicates that the primary mailbox is searched.</span></span> <span data-ttu-id="9d60f-117">Um valor de texto de **ArchiveOnly** indica que a caixa de correio de arquivo morto é pesquisada.</span><span class="sxs-lookup"><span data-stu-id="9d60f-117">A text value of **ArchiveOnly** indicates that the archive mailbox is searched.</span></span> <span data-ttu-id="9d60f-118">Um valor de texto de **todas as** indica que os dois primário e caixas de correio de arquivo morto são pesquisadas.</span><span class="sxs-lookup"><span data-stu-id="9d60f-118">A text value of **All** indicates that both the primary and archive mailboxes are searched.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9d60f-119">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="9d60f-119">Remarks</span></span>

<span data-ttu-id="9d60f-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9d60f-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9d60f-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d60f-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d60f-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9d60f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d60f-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="9d60f-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9d60f-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9d60f-124">Schema name</span></span>  <br/> |<span data-ttu-id="9d60f-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9d60f-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="9d60f-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9d60f-126">Validation file</span></span>  <br/> |<span data-ttu-id="9d60f-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9d60f-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9d60f-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="9d60f-128">Can be empty</span></span>  <br/> ||
   

