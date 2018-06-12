---
title: ResultType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 488ee828-343f-4382-a5e8-eed1005f5dbc
description: O elemento ResultType contém o tipo de pesquisa a ser executado. O tipo de pesquisa pode ser apenas estatísticas ou visualizar apenas.
ms.openlocfilehash: 750f53ae05a7ad9f5aefc9396911a23ef32cdfc2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825211"
---
# <a name="resulttype"></a><span data-ttu-id="35e43-104">ResultType</span><span class="sxs-lookup"><span data-stu-id="35e43-104">ResultType</span></span>

<span data-ttu-id="35e43-105">O elemento **ResultType** contém o tipo de pesquisa a ser executado.</span><span class="sxs-lookup"><span data-stu-id="35e43-105">The **ResultType** element contains the type of search to perform.</span></span> <span data-ttu-id="35e43-106">O tipo de pesquisa pode ser apenas estatísticas ou visualizar apenas.</span><span class="sxs-lookup"><span data-stu-id="35e43-106">The type of search can be statistics only or preview only.</span></span> 
  
```XML
<ResultType>StatisticsOnly | PreviewOnly</ResultType>
```

 <span data-ttu-id="35e43-107">**SearchResultType**</span><span class="sxs-lookup"><span data-stu-id="35e43-107">**SearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="35e43-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="35e43-108">Attributes and elements</span></span>

<span data-ttu-id="35e43-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="35e43-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="35e43-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="35e43-110">Attributes</span></span>

<span data-ttu-id="35e43-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="35e43-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="35e43-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="35e43-112">Child elements</span></span>

<span data-ttu-id="35e43-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="35e43-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="35e43-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="35e43-114">Parent elements</span></span>

<span data-ttu-id="35e43-115">[SearchMailboxesResult](searchmailboxesresult.md) | [SearchMailboxes](searchmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="35e43-115">[SearchMailboxesResult](searchmailboxesresult.md) | [SearchMailboxes](searchmailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="35e43-116">Text value</span><span class="sxs-lookup"><span data-stu-id="35e43-116">Text value</span></span>

<span data-ttu-id="35e43-117">O valor de texto do elemento **ResultType** é o tipo de resultado que é retornado para uma pesquisa de descoberta.</span><span class="sxs-lookup"><span data-stu-id="35e43-117">The text value of the **ResultType** element is the type of result that is returned for a discovery search.</span></span> <span data-ttu-id="35e43-118">Um valor de texto de **StatisticsOnly** retornará as estatísticas da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="35e43-118">A text value of **StatisticsOnly** will return the search statistics.</span></span> <span data-ttu-id="35e43-119">Um valor de texto de **PreviewOnly** irá retornar informações de visualização do item.</span><span class="sxs-lookup"><span data-stu-id="35e43-119">A text value of **PreviewOnly** will return item preview information.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="35e43-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="35e43-120">Remarks</span></span>

<span data-ttu-id="35e43-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="35e43-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="35e43-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="35e43-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="35e43-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="35e43-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="35e43-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="35e43-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="35e43-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="35e43-125">Schema name</span></span>  <br/> |<span data-ttu-id="35e43-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="35e43-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="35e43-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="35e43-127">Validation file</span></span>  <br/> |<span data-ttu-id="35e43-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="35e43-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="35e43-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="35e43-129">Can be empty</span></span>  <br/> |<span data-ttu-id="35e43-130">false</span><span class="sxs-lookup"><span data-stu-id="35e43-130">false</span></span>  <br/> |
   

