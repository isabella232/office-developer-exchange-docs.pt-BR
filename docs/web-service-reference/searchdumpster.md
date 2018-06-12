---
title: SearchDumpster
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddb62dce-c87a-4714-8023-a6b697a29699
description: O elemento SearchDumpster Especifica se deve pesquisar no Dumpster de Exchange.
ms.openlocfilehash: 4a40ee2da7fdaa4eaa3f5349545a0bfd3e13ba73
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825283"
---
# <a name="searchdumpster"></a><span data-ttu-id="7ae5b-103">SearchDumpster</span><span class="sxs-lookup"><span data-stu-id="7ae5b-103">SearchDumpster</span></span>

<span data-ttu-id="7ae5b-104">O elemento **SearchDumpster** Especifica se deve pesquisar no Dumpster de Exchange.</span><span class="sxs-lookup"><span data-stu-id="7ae5b-104">The **SearchDumpster** element specifies whether to search in the Exchange Dumpster.</span></span> 
  
```XML
<SearchDumpster> true | false </SearchDumpster>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="7ae5b-105">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7ae5b-105">Attributes and elements</span></span>

<span data-ttu-id="7ae5b-106">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7ae5b-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ae5b-107">Atributos</span><span class="sxs-lookup"><span data-stu-id="7ae5b-107">Attributes</span></span>

<span data-ttu-id="7ae5b-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7ae5b-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7ae5b-109">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7ae5b-109">Child elements</span></span>

<span data-ttu-id="7ae5b-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7ae5b-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7ae5b-111">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7ae5b-111">Parent elements</span></span>

[<span data-ttu-id="7ae5b-112">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="7ae5b-112">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md)
  
## <a name="text-value"></a><span data-ttu-id="7ae5b-113">Text value</span><span class="sxs-lookup"><span data-stu-id="7ae5b-113">Text value</span></span>

<span data-ttu-id="7ae5b-114">Um valor de texto de **true** para o elemento **SearchDumpster** indica que a pesquisa de estatísticas de caixa de correio inclui o Dumpster de Exchange.</span><span class="sxs-lookup"><span data-stu-id="7ae5b-114">A text value of **true** for the **SearchDumpster** element indicates that the mailbox statistics search includes the Exchange Dumpster.</span></span> <span data-ttu-id="7ae5b-115">Um valor **false** indica que o Dumpster do Exchange não é pesquisado.</span><span class="sxs-lookup"><span data-stu-id="7ae5b-115">A value of **false** indicates that the Exchange Dumpster is not searched.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7ae5b-116">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="7ae5b-116">Remarks</span></span>

<span data-ttu-id="7ae5b-117">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7ae5b-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7ae5b-118">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7ae5b-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ae5b-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7ae5b-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ae5b-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="7ae5b-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7ae5b-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7ae5b-121">Schema name</span></span>  <br/> |<span data-ttu-id="7ae5b-122">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7ae5b-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="7ae5b-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7ae5b-123">Validation file</span></span>  <br/> |<span data-ttu-id="7ae5b-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7ae5b-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7ae5b-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="7ae5b-125">Can be empty</span></span>  <br/> ||
   

