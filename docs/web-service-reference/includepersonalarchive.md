---
title: IncludePersonalArchive
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b373bb1a-6b1d-4959-98a1-4c4ea62973bc
description: O elemento IncludePersonalArchive Especifica se deve incluir o arquivo pessoal na pesquisa.
ms.openlocfilehash: ba2dcaae3befd3595815c7281858e4fa8a738e0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823905"
---
# <a name="includepersonalarchive"></a><span data-ttu-id="fb903-103">IncludePersonalArchive</span><span class="sxs-lookup"><span data-stu-id="fb903-103">IncludePersonalArchive</span></span>

<span data-ttu-id="fb903-104">O elemento **IncludePersonalArchive** Especifica se deve incluir o arquivo pessoal na pesquisa.</span><span class="sxs-lookup"><span data-stu-id="fb903-104">The **IncludePersonalArchive** element specifies whether to include the personal archive in the search.</span></span> 
  
```XML
<IncludePersonalArchive>true | false</IncludePersonalArchive>
```

 <span data-ttu-id="fb903-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="fb903-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb903-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="fb903-106">Attributes and elements</span></span>

<span data-ttu-id="fb903-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fb903-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb903-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fb903-108">Attributes</span></span>

<span data-ttu-id="fb903-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fb903-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb903-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fb903-110">Child elements</span></span>

<span data-ttu-id="fb903-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fb903-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fb903-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fb903-112">Parent elements</span></span>

|<span data-ttu-id="fb903-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fb903-113">**Element**</span></span>|<span data-ttu-id="fb903-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fb903-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb903-115">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="fb903-115">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md) <br/> |<span data-ttu-id="fb903-116">Especifica uma solicitação para pesquisar por palavra-chave estatísticas de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fb903-116">Specifies a request to search for mailbox statistics by keyword.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fb903-117">Text value</span><span class="sxs-lookup"><span data-stu-id="fb903-117">Text value</span></span>

<span data-ttu-id="fb903-118">Um valor de texto de **true** para o elemento **IncludePersonalArchive** indica que o arquivo pessoal é incluído na pesquisa.</span><span class="sxs-lookup"><span data-stu-id="fb903-118">A text value of **true** for the **IncludePersonalArchive** element indicates that the personal archive is included in the search.</span></span> <span data-ttu-id="fb903-119">Um valor **false** indica que o arquivo pessoal não está incluído na pesquisa.</span><span class="sxs-lookup"><span data-stu-id="fb903-119">A value of **false** indicates that the personal archive is not included in the search.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fb903-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="fb903-120">Remarks</span></span>

<span data-ttu-id="fb903-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb903-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb903-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="fb903-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb903-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="fb903-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fb903-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fb903-124">Schema Name</span></span>  <br/> |<span data-ttu-id="fb903-125">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="fb903-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="fb903-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fb903-126">Validation File</span></span>  <br/> |<span data-ttu-id="fb903-127">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fb903-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fb903-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="fb903-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="fb903-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="fb903-129">See also</span></span>



- [<span data-ttu-id="fb903-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fb903-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

