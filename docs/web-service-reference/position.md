---
title: Posição
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46726ebb-a403-4793-8378-282aa7dc39d0
description: O elemento position especifica a posição de uma entidade extraída de uma mensagem.
ms.openlocfilehash: 9acd965c3e0c29f3fa91df338c0671749192b38b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465419"
---
# <a name="position"></a><span data-ttu-id="05540-103">Posição</span><span class="sxs-lookup"><span data-stu-id="05540-103">Position</span></span>

<span data-ttu-id="05540-104">O elemento **Position** especifica a posição de uma entidade extraída de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="05540-104">The **Position** element specifies the position of an entity extracted from a message.</span></span> 
  
```XML
<Position> LatestReply | Other | Subject | Signature </Position>
```

 <span data-ttu-id="05540-105">**EmailPositionType**</span><span class="sxs-lookup"><span data-stu-id="05540-105">**EmailPositionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05540-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="05540-106">Attributes and elements</span></span>

<span data-ttu-id="05540-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="05540-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05540-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="05540-108">Attributes</span></span>

<span data-ttu-id="05540-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="05540-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05540-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="05540-110">Child elements</span></span>

<span data-ttu-id="05540-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="05540-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="05540-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="05540-112">Parent elements</span></span>

<span data-ttu-id="05540-113">[UrlEntity](urlentity.md)  |  [AddressEntity](addressentity.md)  |  [EmailAddressEntity](emailaddressentity.md)  |  [MeetingSuggestion](meetingsuggestion.md)  |  [Contato (ContactType)](contact-contacttype.md)  |  [Telefone (PhoneEntityType)](phone-phoneentitytype.md)  |  [TaskSuggestion](tasksuggestion.md)</span><span class="sxs-lookup"><span data-stu-id="05540-113">[UrlEntity](urlentity.md) | [AddressEntity](addressentity.md) | [EmailAddressEntity](emailaddressentity.md) | [MeetingSuggestion](meetingsuggestion.md) | [Contact (ContactType)](contact-contacttype.md) | [Phone (PhoneEntityType)](phone-phoneentitytype.md) | [TaskSuggestion](tasksuggestion.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="05540-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="05540-114">Text value</span></span>

<span data-ttu-id="05540-115">O valor de texto do elemento **Position** é o local onde uma entidade extraída originou a mensagem de origem.</span><span class="sxs-lookup"><span data-stu-id="05540-115">The text value of the **Position** element is the location where an extracted entity originated in the source message.</span></span> <span data-ttu-id="05540-116">Os valores de texto para o elemento **Position** são:</span><span class="sxs-lookup"><span data-stu-id="05540-116">The text values for the **Position** element are:</span></span> 
  
- <span data-ttu-id="05540-117">**LatestReply** -a entidade extraída se origina da resposta mais recente à mensagem.</span><span class="sxs-lookup"><span data-stu-id="05540-117">**LatestReply** - the extracted entity originates from the latest reply to the message.</span></span> 
    
- <span data-ttu-id="05540-118">**Other** -a entidade extraída é originada de uma parte indefinida da mensagem.</span><span class="sxs-lookup"><span data-stu-id="05540-118">**Other** - the extracted entity originates from an undefined part of the message.</span></span> 
    
- <span data-ttu-id="05540-119">**Subject** -a entidade extraída é originada do assunto da mensagem.</span><span class="sxs-lookup"><span data-stu-id="05540-119">**Subject** - the extracted entity originates from the message subject.</span></span> 
    
- <span data-ttu-id="05540-120">**Signature** -a entidade extraída provém da assinatura da mensagem.</span><span class="sxs-lookup"><span data-stu-id="05540-120">**Signature** - the extracted entity originates from the message signature.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="05540-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="05540-121">Remarks</span></span>

<span data-ttu-id="05540-122">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="05540-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="05540-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="05540-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05540-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="05540-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05540-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="05540-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05540-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="05540-126">Schema name</span></span>  <br/> |<span data-ttu-id="05540-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="05540-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="05540-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="05540-128">Validation file</span></span>  <br/> |<span data-ttu-id="05540-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="05540-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="05540-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="05540-130">Can be empty</span></span>  <br/> ||
   

