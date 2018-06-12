---
title: HasAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: de152be6-fc2f-48bc-a05d-1211935da20a
description: O elemento HasAttachment Especifica um valor booleano para indicar se o item tem anexos.
ms.openlocfilehash: dfe163e0850e835784a43984a34c89f14bfbc59b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823798"
---
# <a name="hasattachment"></a><span data-ttu-id="059f4-103">HasAttachment</span><span class="sxs-lookup"><span data-stu-id="059f4-103">HasAttachment</span></span>

<span data-ttu-id="059f4-104">O elemento **HasAttachment** Especifica um valor booleano para indicar se o item tem anexos.</span><span class="sxs-lookup"><span data-stu-id="059f4-104">The **HasAttachment** element specifies a Boolean value to indicate whether the item has attachments.</span></span> 
  
```XML
<HasAttachment> true | false </HasAttachment
```

 <span data-ttu-id="059f4-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="059f4-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="059f4-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="059f4-106">Attributes and elements</span></span>

<span data-ttu-id="059f4-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="059f4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="059f4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="059f4-108">Attributes</span></span>

<span data-ttu-id="059f4-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="059f4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="059f4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="059f4-110">Child elements</span></span>

<span data-ttu-id="059f4-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="059f4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="059f4-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="059f4-112">Parent elements</span></span>

|<span data-ttu-id="059f4-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="059f4-113">**Element**</span></span>|<span data-ttu-id="059f4-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="059f4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="059f4-115">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="059f4-115">SearchPreviewItem</span></span>](searchpreviewitem.md) <br/> |<span data-ttu-id="059f4-116">Especifica os primeiros 256 caracteres de um item de caixa de correio para visualização sem abrir o item.</span><span class="sxs-lookup"><span data-stu-id="059f4-116">Specifies the first 256 characters of a mailbox item for preview without opening the item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="059f4-117">Text value</span><span class="sxs-lookup"><span data-stu-id="059f4-117">Text value</span></span>

<span data-ttu-id="059f4-118">Um valor de **true** para o elemento **HasAttachment** text indica que o item tiver um anexo.</span><span class="sxs-lookup"><span data-stu-id="059f4-118">A text value of **true** for the **HasAttachment** element indicates that the item has an attachment.</span></span> <span data-ttu-id="059f4-119">Um valor **false** indica que o item não tiver um anexo.</span><span class="sxs-lookup"><span data-stu-id="059f4-119">A value of **false** indicates that the item does not have an attachment.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="059f4-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="059f4-120">Remarks</span></span>

<span data-ttu-id="059f4-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="059f4-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="059f4-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="059f4-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="059f4-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="059f4-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="059f4-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="059f4-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="059f4-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="059f4-125">Schema Name</span></span>  <br/> |<span data-ttu-id="059f4-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="059f4-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="059f4-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="059f4-127">Validation File</span></span>  <br/> |<span data-ttu-id="059f4-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="059f4-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="059f4-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="059f4-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="059f4-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="059f4-130">See also</span></span>



- [<span data-ttu-id="059f4-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="059f4-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

