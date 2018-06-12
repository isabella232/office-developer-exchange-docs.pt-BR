---
title: HasLocationChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5fd465b4-6070-4cd0-9ac3-ed9d2bfd5951
description: O elemento HasLocationChanged Especifica se a propriedade location de uma reunião foi alterada.
ms.openlocfilehash: dbb811b93149be0bb43fbb2f579a5086a396e401
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823804"
---
# <a name="haslocationchanged"></a><span data-ttu-id="9fd92-103">HasLocationChanged</span><span class="sxs-lookup"><span data-stu-id="9fd92-103">HasLocationChanged</span></span>

<span data-ttu-id="9fd92-104">O elemento **HasLocationChanged** Especifica se a propriedade location de uma reunião foi alterada.</span><span class="sxs-lookup"><span data-stu-id="9fd92-104">The **HasLocationChanged** element specifies whether the location property of a meeting has changed.</span></span> 
  
```XML
<HasLocationChanged> true | false </HasLocationChanged>
```

 <span data-ttu-id="9fd92-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="9fd92-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9fd92-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9fd92-106">Attributes and elements</span></span>

<span data-ttu-id="9fd92-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9fd92-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9fd92-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9fd92-108">Attributes</span></span>

<span data-ttu-id="9fd92-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9fd92-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9fd92-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9fd92-110">Child elements</span></span>

<span data-ttu-id="9fd92-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9fd92-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9fd92-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9fd92-112">Parent elements</span></span>

|<span data-ttu-id="9fd92-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9fd92-113">**Element**</span></span>|<span data-ttu-id="9fd92-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9fd92-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9fd92-115">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="9fd92-115">ChangeHighlights</span></span>](changehighlights.md) <br/> |<span data-ttu-id="9fd92-116">Especifica o que mudou entre duas versões de uma reunião mensagem de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9fd92-116">Specifies what has changed between two versions of a meeting request message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9fd92-117">Text value</span><span class="sxs-lookup"><span data-stu-id="9fd92-117">Text value</span></span>

<span data-ttu-id="9fd92-118">Um valor de texto de **true** para o elemento **HasLocationChanged** indica que a propriedade location de uma reunião foi alterado.</span><span class="sxs-lookup"><span data-stu-id="9fd92-118">A text value of **true** for the **HasLocationChanged** element indicates that the location property of a meeting has changed.</span></span> <span data-ttu-id="9fd92-119">Um valor **false** indica que a propriedade location de uma reunião não tiver sido alterado.</span><span class="sxs-lookup"><span data-stu-id="9fd92-119">A value **false** indicates that the location property of a meeting has not changed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9fd92-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="9fd92-120">Remarks</span></span>

<span data-ttu-id="9fd92-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9fd92-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9fd92-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fd92-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9fd92-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9fd92-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9fd92-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="9fd92-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9fd92-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9fd92-125">Schema Name</span></span>  <br/> |<span data-ttu-id="9fd92-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="9fd92-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="9fd92-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9fd92-127">Validation File</span></span>  <br/> |<span data-ttu-id="9fd92-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9fd92-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9fd92-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="9fd92-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9fd92-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="9fd92-130">See also</span></span>



- [<span data-ttu-id="9fd92-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9fd92-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

