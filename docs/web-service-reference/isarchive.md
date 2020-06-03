---
title: IsArchive
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b89d8a78-5c18-4547-aaf4-4b16a93190a7
description: O elemento IsArchive especifica um valor Boolean que indica se a caixa de correio é uma caixa de correio de arquivo morto.
ms.openlocfilehash: 6d0be0eb283de3f4d8f786ff96f4a0d4f49e2009
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526512"
---
# <a name="isarchive"></a><span data-ttu-id="5f3f2-103">IsArchive</span><span class="sxs-lookup"><span data-stu-id="5f3f2-103">IsArchive</span></span>

<span data-ttu-id="5f3f2-104">O elemento **IsArchive** especifica um valor Boolean que indica se a caixa de correio é uma caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="5f3f2-104">The **IsArchive** element specifies a Boolean value that indicates whether the mailbox is an archive mailbox.</span></span> 
  
```XML
<IsArchive>true | false</IsArchive>
```

 <span data-ttu-id="5f3f2-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="5f3f2-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5f3f2-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5f3f2-106">Attributes and elements</span></span>

<span data-ttu-id="5f3f2-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5f3f2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5f3f2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5f3f2-108">Attributes</span></span>

<span data-ttu-id="5f3f2-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5f3f2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5f3f2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5f3f2-110">Child elements</span></span>

<span data-ttu-id="5f3f2-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5f3f2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5f3f2-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5f3f2-112">Parent elements</span></span>

<span data-ttu-id="5f3f2-113">[FailedMailbox](failedmailbox.md)  |  [RetentionPolicyTag](retentionpolicytag.md)</span><span class="sxs-lookup"><span data-stu-id="5f3f2-113">[FailedMailbox](failedmailbox.md) | [RetentionPolicyTag](retentionpolicytag.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="5f3f2-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5f3f2-114">Text value</span></span>

<span data-ttu-id="5f3f2-115">Um valor de texto **true** para o elemento **IsArchive** indica que a caixa de correio de destino é uma caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="5f3f2-115">A text value of **true** for the **IsArchive** element indicates that the target mailbox is an archive mailbox.</span></span> <span data-ttu-id="5f3f2-116">Um valor **false** indica que a caixa de correio de destino não é uma caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="5f3f2-116">A value of **false** indicates that the target mailbox is not an archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5f3f2-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="5f3f2-117">Remarks</span></span>

<span data-ttu-id="5f3f2-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5f3f2-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5f3f2-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f3f2-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5f3f2-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5f3f2-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5f3f2-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="5f3f2-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5f3f2-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5f3f2-122">Schema Name</span></span>  <br/> |<span data-ttu-id="5f3f2-123">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="5f3f2-123">Type schema</span></span>  <br/> |
|<span data-ttu-id="5f3f2-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5f3f2-124">Validation File</span></span>  <br/> |<span data-ttu-id="5f3f2-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5f3f2-125">types.xsd</span></span>  <br/> |
|<span data-ttu-id="5f3f2-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="5f3f2-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="5f3f2-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="5f3f2-127">See also</span></span>



- [<span data-ttu-id="5f3f2-128">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5f3f2-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

