---
title: ResultType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 488ee828-343f-4382-a5e8-eed1005f5dbc
description: O elemento ResultType contém o tipo de pesquisa a ser executada. O tipo de pesquisa pode ser apenas estatísticas ou apenas visualização.
ms.openlocfilehash: 6617c8b4b64cd9b6728317d7247bcc5378e488f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465279"
---
# <a name="resulttype"></a><span data-ttu-id="6cbe9-104">ResultType</span><span class="sxs-lookup"><span data-stu-id="6cbe9-104">ResultType</span></span>

<span data-ttu-id="6cbe9-105">O elemento **ResultType** contém o tipo de pesquisa a ser executada.</span><span class="sxs-lookup"><span data-stu-id="6cbe9-105">The **ResultType** element contains the type of search to perform.</span></span> <span data-ttu-id="6cbe9-106">O tipo de pesquisa pode ser apenas estatísticas ou apenas visualização.</span><span class="sxs-lookup"><span data-stu-id="6cbe9-106">The type of search can be statistics only or preview only.</span></span> 
  
```XML
<ResultType>StatisticsOnly | PreviewOnly</ResultType>
```

 <span data-ttu-id="6cbe9-107">**SearchResulttype**</span><span class="sxs-lookup"><span data-stu-id="6cbe9-107">**SearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6cbe9-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6cbe9-108">Attributes and elements</span></span>

<span data-ttu-id="6cbe9-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6cbe9-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6cbe9-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="6cbe9-110">Attributes</span></span>

<span data-ttu-id="6cbe9-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6cbe9-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6cbe9-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6cbe9-112">Child elements</span></span>

<span data-ttu-id="6cbe9-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6cbe9-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6cbe9-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6cbe9-114">Parent elements</span></span>

<span data-ttu-id="6cbe9-115">[SearchMailboxesResult](searchmailboxesresult.md)  |  [SearchMailboxes](searchmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="6cbe9-115">[SearchMailboxesResult](searchmailboxesresult.md) | [SearchMailboxes](searchmailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="6cbe9-116">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="6cbe9-116">Text value</span></span>

<span data-ttu-id="6cbe9-117">O valor de texto do elemento **ResultType** é o tipo de resultado que é retornado para uma pesquisa de descoberta.</span><span class="sxs-lookup"><span data-stu-id="6cbe9-117">The text value of the **ResultType** element is the type of result that is returned for a discovery search.</span></span> <span data-ttu-id="6cbe9-118">Um valor de texto de **StatisticsOnly** retornará as estatísticas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6cbe9-118">A text value of **StatisticsOnly** will return the search statistics.</span></span> <span data-ttu-id="6cbe9-119">Um valor de texto de **PreviewOnly** retornará informações de visualização do item.</span><span class="sxs-lookup"><span data-stu-id="6cbe9-119">A text value of **PreviewOnly** will return item preview information.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6cbe9-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="6cbe9-120">Remarks</span></span>

<span data-ttu-id="6cbe9-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6cbe9-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6cbe9-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6cbe9-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6cbe9-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6cbe9-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6cbe9-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="6cbe9-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6cbe9-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6cbe9-125">Schema name</span></span>  <br/> |<span data-ttu-id="6cbe9-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="6cbe9-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6cbe9-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6cbe9-127">Validation file</span></span>  <br/> |<span data-ttu-id="6cbe9-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6cbe9-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6cbe9-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="6cbe9-129">Can be empty</span></span>  <br/> |<span data-ttu-id="6cbe9-130">falso</span><span class="sxs-lookup"><span data-stu-id="6cbe9-130">false</span></span>  <br/> |
   

