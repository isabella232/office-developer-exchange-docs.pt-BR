---
title: HasLocationChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5fd465b4-6070-4cd0-9ac3-ed9d2bfd5951
description: O elemento HasLocationChanged especifica se a propriedade Location de uma reunião foi alterada.
ms.openlocfilehash: 4f774adcf4a7666f40524931504f1172e15ba24d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462441"
---
# <a name="haslocationchanged"></a><span data-ttu-id="54dfd-103">HasLocationChanged</span><span class="sxs-lookup"><span data-stu-id="54dfd-103">HasLocationChanged</span></span>

<span data-ttu-id="54dfd-104">O elemento **HasLocationChanged** especifica se a propriedade Location de uma reunião foi alterada.</span><span class="sxs-lookup"><span data-stu-id="54dfd-104">The **HasLocationChanged** element specifies whether the location property of a meeting has changed.</span></span> 
  
```XML
<HasLocationChanged> true | false </HasLocationChanged>
```

 <span data-ttu-id="54dfd-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="54dfd-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54dfd-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="54dfd-106">Attributes and elements</span></span>

<span data-ttu-id="54dfd-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="54dfd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54dfd-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="54dfd-108">Attributes</span></span>

<span data-ttu-id="54dfd-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="54dfd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54dfd-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="54dfd-110">Child elements</span></span>

<span data-ttu-id="54dfd-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="54dfd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="54dfd-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="54dfd-112">Parent elements</span></span>

|<span data-ttu-id="54dfd-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="54dfd-113">**Element**</span></span>|<span data-ttu-id="54dfd-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="54dfd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54dfd-115">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="54dfd-115">ChangeHighlights</span></span>](changehighlights.md) <br/> |<span data-ttu-id="54dfd-116">Especifica o que mudou entre duas versões de uma mensagem de solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="54dfd-116">Specifies what has changed between two versions of a meeting request message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="54dfd-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="54dfd-117">Text value</span></span>

<span data-ttu-id="54dfd-118">Um valor de texto **true** para o elemento **HasLocationChanged** indica que a propriedade Location de uma reunião foi alterada.</span><span class="sxs-lookup"><span data-stu-id="54dfd-118">A text value of **true** for the **HasLocationChanged** element indicates that the location property of a meeting has changed.</span></span> <span data-ttu-id="54dfd-119">Um valor **false** indica que a propriedade Location de uma reunião não foi alterada.</span><span class="sxs-lookup"><span data-stu-id="54dfd-119">A value **false** indicates that the location property of a meeting has not changed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="54dfd-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="54dfd-120">Remarks</span></span>

<span data-ttu-id="54dfd-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="54dfd-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="54dfd-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="54dfd-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54dfd-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="54dfd-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54dfd-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="54dfd-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="54dfd-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="54dfd-125">Schema Name</span></span>  <br/> |<span data-ttu-id="54dfd-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="54dfd-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="54dfd-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="54dfd-127">Validation File</span></span>  <br/> |<span data-ttu-id="54dfd-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="54dfd-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="54dfd-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="54dfd-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="54dfd-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="54dfd-130">See also</span></span>



- [<span data-ttu-id="54dfd-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="54dfd-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

