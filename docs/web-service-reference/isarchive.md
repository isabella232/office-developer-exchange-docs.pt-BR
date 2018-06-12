---
title: IsArchive
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b89d8a78-5c18-4547-aaf4-4b16a93190a7
description: O elemento IsArchive Especifica um valor Boolean que indica se a caixa de correio é uma caixa de correio de arquivo morto.
ms.openlocfilehash: 417afd1afc25e5872d1f511feff34494fe6b7b62
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823990"
---
# <a name="isarchive"></a><span data-ttu-id="b5667-103">IsArchive</span><span class="sxs-lookup"><span data-stu-id="b5667-103">IsArchive</span></span>

<span data-ttu-id="b5667-104">O elemento **IsArchive** Especifica um valor Boolean que indica se a caixa de correio é uma caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="b5667-104">The **IsArchive** element specifies a Boolean value that indicates whether the mailbox is an archive mailbox.</span></span> 
  
```XML
<IsArchive>true | false</IsArchive>
```

 <span data-ttu-id="b5667-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="b5667-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b5667-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b5667-106">Attributes and elements</span></span>

<span data-ttu-id="b5667-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b5667-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b5667-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b5667-108">Attributes</span></span>

<span data-ttu-id="b5667-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b5667-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b5667-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b5667-110">Child elements</span></span>

<span data-ttu-id="b5667-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b5667-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b5667-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b5667-112">Parent elements</span></span>

<span data-ttu-id="b5667-113">[FailedMailbox](failedmailbox.md) | [RetentionPolicyTag](retentionpolicytag.md)</span><span class="sxs-lookup"><span data-stu-id="b5667-113">[FailedMailbox](failedmailbox.md) | [RetentionPolicyTag](retentionpolicytag.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b5667-114">Text value</span><span class="sxs-lookup"><span data-stu-id="b5667-114">Text value</span></span>

<span data-ttu-id="b5667-115">Um valor de texto de **true** para o elemento **IsArchive** indica que a caixa de correio de destino é uma caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="b5667-115">A text value of **true** for the **IsArchive** element indicates that the target mailbox is an archive mailbox.</span></span> <span data-ttu-id="b5667-116">Um valor **false** indica que a caixa de correio de destino não é uma caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="b5667-116">A value of **false** indicates that the target mailbox is not an archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b5667-117">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="b5667-117">Remarks</span></span>

<span data-ttu-id="b5667-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b5667-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b5667-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5667-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b5667-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b5667-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b5667-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="b5667-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b5667-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b5667-122">Schema Name</span></span>  <br/> |<span data-ttu-id="b5667-123">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="b5667-123">Type schema</span></span>  <br/> |
|<span data-ttu-id="b5667-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b5667-124">Validation File</span></span>  <br/> |<span data-ttu-id="b5667-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b5667-125">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b5667-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b5667-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b5667-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="b5667-127">See also</span></span>



- [<span data-ttu-id="b5667-128">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b5667-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

