---
title: Posição
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46726ebb-a403-4793-8378-282aa7dc39d0
description: O elemento de posição Especifica a posição de uma entidade extraída de uma mensagem.
ms.openlocfilehash: 4bd8f3088891e918e13d5ef1ec8e3e5217cb3fa1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824853"
---
# <a name="position"></a><span data-ttu-id="6730f-103">Posição</span><span class="sxs-lookup"><span data-stu-id="6730f-103">Position</span></span>

<span data-ttu-id="6730f-104">O elemento de **posição** Especifica a posição de uma entidade extraída de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="6730f-104">The **Position** element specifies the position of an entity extracted from a message.</span></span> 
  
```XML
<Position> LatestReply | Other | Subject | Signature </Position>
```

 <span data-ttu-id="6730f-105">**EmailPositionType**</span><span class="sxs-lookup"><span data-stu-id="6730f-105">**EmailPositionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6730f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6730f-106">Attributes and elements</span></span>

<span data-ttu-id="6730f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6730f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6730f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6730f-108">Attributes</span></span>

<span data-ttu-id="6730f-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6730f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6730f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6730f-110">Child elements</span></span>

<span data-ttu-id="6730f-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6730f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6730f-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6730f-112">Parent elements</span></span>

<span data-ttu-id="6730f-113">[UrlEntity](urlentity.md) | [AddressEntity](addressentity.md) | [EmailAddressEntity](emailaddressentity.md) | [MeetingSuggestion](meetingsuggestion.md) | [contato (ContactType)](contact-contacttype.md) | [telefone (PhoneEntityType)](phone-phoneentitytype.md)  |  [ TaskSuggestion](tasksuggestion.md)</span><span class="sxs-lookup"><span data-stu-id="6730f-113">[UrlEntity](urlentity.md) | [AddressEntity](addressentity.md) | [EmailAddressEntity](emailaddressentity.md) | [MeetingSuggestion](meetingsuggestion.md) | [Contact (ContactType)](contact-contacttype.md) | [Phone (PhoneEntityType)](phone-phoneentitytype.md) | [TaskSuggestion](tasksuggestion.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="6730f-114">Text value</span><span class="sxs-lookup"><span data-stu-id="6730f-114">Text value</span></span>

<span data-ttu-id="6730f-115">O valor de texto do elemento **posição** é o local onde uma entidade extraída originou na mensagem de origem.</span><span class="sxs-lookup"><span data-stu-id="6730f-115">The text value of the **Position** element is the location where an extracted entity originated in the source message.</span></span> <span data-ttu-id="6730f-116">Os valores de texto para o elemento de **posição** são:</span><span class="sxs-lookup"><span data-stu-id="6730f-116">The text values for the **Position** element are:</span></span> 
  
- <span data-ttu-id="6730f-117">**LatestReply** - a entidade extraída se origina a resposta mais recente à mensagem.</span><span class="sxs-lookup"><span data-stu-id="6730f-117">**LatestReply** - the extracted entity originates from the latest reply to the message.</span></span> 
    
- <span data-ttu-id="6730f-118">**Outros** - a entidade extraída originado de uma indefinido parte da mensagem.</span><span class="sxs-lookup"><span data-stu-id="6730f-118">**Other** - the extracted entity originates from an undefined part of the message.</span></span> 
    
- <span data-ttu-id="6730f-119">**Assunto** - a entidade extraída originado de assunto da mensagem.</span><span class="sxs-lookup"><span data-stu-id="6730f-119">**Subject** - the extracted entity originates from the message subject.</span></span> 
    
- <span data-ttu-id="6730f-120">**Assinatura** - a entidade extraída se origina a assinatura da mensagem.</span><span class="sxs-lookup"><span data-stu-id="6730f-120">**Signature** - the extracted entity originates from the message signature.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="6730f-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="6730f-121">Remarks</span></span>

<span data-ttu-id="6730f-122">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6730f-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6730f-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6730f-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6730f-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6730f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6730f-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="6730f-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6730f-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6730f-126">Schema name</span></span>  <br/> |<span data-ttu-id="6730f-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6730f-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="6730f-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6730f-128">Validation file</span></span>  <br/> |<span data-ttu-id="6730f-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6730f-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6730f-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="6730f-130">Can be empty</span></span>  <br/> ||
   

