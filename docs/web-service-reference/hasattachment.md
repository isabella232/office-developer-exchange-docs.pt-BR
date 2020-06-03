---
title: HasAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: de152be6-fc2f-48bc-a05d-1211935da20a
description: O elemento HasAttachment especifica um valor Boolean para indicar se o item tem anexos.
ms.openlocfilehash: c6bc0932a08a1bbec215bb8a974ed746d2961123
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530258"
---
# <a name="hasattachment"></a><span data-ttu-id="8171c-103">HasAttachment</span><span class="sxs-lookup"><span data-stu-id="8171c-103">HasAttachment</span></span>

<span data-ttu-id="8171c-104">O elemento **HasAttachment** especifica um valor Boolean para indicar se o item tem anexos.</span><span class="sxs-lookup"><span data-stu-id="8171c-104">The **HasAttachment** element specifies a Boolean value to indicate whether the item has attachments.</span></span> 
  
```XML
<HasAttachment> true | false </HasAttachment
```

 <span data-ttu-id="8171c-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="8171c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8171c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8171c-106">Attributes and elements</span></span>

<span data-ttu-id="8171c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8171c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8171c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8171c-108">Attributes</span></span>

<span data-ttu-id="8171c-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8171c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8171c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8171c-110">Child elements</span></span>

<span data-ttu-id="8171c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8171c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8171c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8171c-112">Parent elements</span></span>

|<span data-ttu-id="8171c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8171c-113">**Element**</span></span>|<span data-ttu-id="8171c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8171c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8171c-115">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="8171c-115">SearchPreviewItem</span></span>](searchpreviewitem.md) <br/> |<span data-ttu-id="8171c-116">Especifica os primeiros 256 caracteres de um item de caixa de correio para visualização sem abrir o item.</span><span class="sxs-lookup"><span data-stu-id="8171c-116">Specifies the first 256 characters of a mailbox item for preview without opening the item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8171c-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="8171c-117">Text value</span></span>

<span data-ttu-id="8171c-118">Um valor de texto **true** para o elemento **HasAttachment** indica que o item tem um anexo.</span><span class="sxs-lookup"><span data-stu-id="8171c-118">A text value of **true** for the **HasAttachment** element indicates that the item has an attachment.</span></span> <span data-ttu-id="8171c-119">Um valor **false** indica que o item não tem um anexo.</span><span class="sxs-lookup"><span data-stu-id="8171c-119">A value of **false** indicates that the item does not have an attachment.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8171c-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="8171c-120">Remarks</span></span>

<span data-ttu-id="8171c-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8171c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8171c-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8171c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8171c-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8171c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8171c-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="8171c-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8171c-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8171c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="8171c-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="8171c-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="8171c-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8171c-127">Validation File</span></span>  <br/> |<span data-ttu-id="8171c-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8171c-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="8171c-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="8171c-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="8171c-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="8171c-130">See also</span></span>



- [<span data-ttu-id="8171c-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8171c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

