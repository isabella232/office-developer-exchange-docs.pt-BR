---
title: GetSearchableMailboxesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0fcc2f53-742b-46ae-bbab-c3295a3d69e7
description: O elemento GetSearchableMailboxesResponse contém a resposta a uma solicitação GetSearchableMailboxes.
ms.openlocfilehash: 35a671cd534d1b48b29ef836c24d97d7cbd52401
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752624"
---
# <a name="getsearchablemailboxesresponse"></a><span data-ttu-id="02c4c-103">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="02c4c-103">GetSearchableMailboxesResponse</span></span>

<span data-ttu-id="02c4c-104">O elemento **GetSearchableMailboxesResponse** contém a resposta a uma solicitação **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="02c4c-104">The **GetSearchableMailboxesResponse** element contains the response to a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<GetSearchableMailboxesResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SearchableMailboxes/>
   <FailedMailboxes/>
</GetSearchableMailboxesResponse>
```

 <span data-ttu-id="02c4c-105">**GetSearchableMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="02c4c-105">**GetSearchableMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="02c4c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="02c4c-106">Attributes and elements</span></span>

<span data-ttu-id="02c4c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="02c4c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02c4c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="02c4c-108">Attributes</span></span>

<span data-ttu-id="02c4c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="02c4c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="02c4c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="02c4c-110">Child elements</span></span>

<span data-ttu-id="02c4c-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [SearchableMailboxes](searchablemailboxes.md) | [FailedMailboxes](failedmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="02c4c-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [SearchableMailboxes](searchablemailboxes.md) | [FailedMailboxes](failedmailboxes.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="02c4c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="02c4c-112">Parent elements</span></span>

<span data-ttu-id="02c4c-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="02c4c-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="02c4c-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="02c4c-114">Remarks</span></span>

<span data-ttu-id="02c4c-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="02c4c-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="02c4c-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="02c4c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="02c4c-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="02c4c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02c4c-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="02c4c-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="02c4c-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="02c4c-119">Schema name</span></span>  <br/> |<span data-ttu-id="02c4c-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="02c4c-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="02c4c-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="02c4c-121">Validation file</span></span>  <br/> |<span data-ttu-id="02c4c-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="02c4c-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="02c4c-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="02c4c-123">Can be empty</span></span>  <br/> |<span data-ttu-id="02c4c-124">false</span><span class="sxs-lookup"><span data-stu-id="02c4c-124">false</span></span>  <br/> |
   

