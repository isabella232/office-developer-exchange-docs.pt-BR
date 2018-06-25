---
title: ArchiveItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 68109a92-c49e-4c0e-b6ec-e90d38d4be4d
description: O elemento ArchiveItemResponse Especifica a resposta a uma solicitação ArchiveItem.
ms.openlocfilehash: bfd1b9d76c2b49e00a82bd8f6f57742007d0adf7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751199"
---
# <a name="archiveitemresponse"></a><span data-ttu-id="4e1a9-103">ArchiveItemResponse</span><span class="sxs-lookup"><span data-stu-id="4e1a9-103">ArchiveItemResponse</span></span>

<span data-ttu-id="4e1a9-104">O elemento **ArchiveItemResponse** Especifica a resposta a uma solicitação **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="4e1a9-104">The **ArchiveItemResponse** element specifies the response to an **ArchiveItem** request.</span></span> 
  
```XML
<ArchiveItemResponse>
    <ResponseMessages></ResponseMessages>
</ArchiveItemResponse>
```

 <span data-ttu-id="4e1a9-105">**ArchiveItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="4e1a9-105">**ArchiveItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4e1a9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4e1a9-106">Attributes and elements</span></span>

<span data-ttu-id="4e1a9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4e1a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4e1a9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4e1a9-108">Attributes</span></span>

<span data-ttu-id="4e1a9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4e1a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4e1a9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4e1a9-110">Child elements</span></span>

|<span data-ttu-id="4e1a9-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4e1a9-111">**Element**</span></span>|<span data-ttu-id="4e1a9-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4e1a9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e1a9-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4e1a9-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="4e1a9-114">Contém as mensagens de resposta a uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e1a9-114">Contains the response messages to an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4e1a9-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4e1a9-115">Parent elements</span></span>

<span data-ttu-id="4e1a9-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4e1a9-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4e1a9-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="4e1a9-117">Remarks</span></span>

<span data-ttu-id="4e1a9-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4e1a9-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4e1a9-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e1a9-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4e1a9-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4e1a9-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4e1a9-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="4e1a9-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4e1a9-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4e1a9-122">Schema Name</span></span>  <br/> |<span data-ttu-id="4e1a9-123">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="4e1a9-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="4e1a9-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4e1a9-124">Validation File</span></span>  <br/> |<span data-ttu-id="4e1a9-125">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4e1a9-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4e1a9-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="4e1a9-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4e1a9-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="4e1a9-127">See also</span></span>

- [<span data-ttu-id="4e1a9-128">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4e1a9-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

