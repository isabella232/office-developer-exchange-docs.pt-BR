---
title: MakeItemImmutable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: de1d2a60-aeeb-4625-8b11-23c42e1e7bae
description: O elemento MakeItemImmutable Especifica um valor Boolean que indica se um item deve ser feito somente leitura.
ms.openlocfilehash: 63c05fd3572c7b4ab93fe098d9165a117849ef02
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824337"
---
# <a name="makeitemimmutable"></a><span data-ttu-id="5c857-103">MakeItemImmutable</span><span class="sxs-lookup"><span data-stu-id="5c857-103">MakeItemImmutable</span></span>

<span data-ttu-id="5c857-104">O elemento **MakeItemImmutable** Especifica um valor Boolean que indica se um item deve ser feito somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5c857-104">The **MakeItemImmutable** element specifies a Boolean value that indicates whether an item should be made read-only.</span></span> 
  
```XML
<MakeItemImmutable>true | false</MakeItemImmutable>
```

 <span data-ttu-id="5c857-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="5c857-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c857-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5c857-106">Attributes and elements</span></span>

<span data-ttu-id="5c857-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5c857-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c857-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5c857-108">Attributes</span></span>

<span data-ttu-id="5c857-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5c857-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c857-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5c857-110">Child elements</span></span>

<span data-ttu-id="5c857-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5c857-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5c857-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5c857-112">Parent elements</span></span>

[<span data-ttu-id="5c857-113">UpdateItemInRecoverableItems</span><span class="sxs-lookup"><span data-stu-id="5c857-113">UpdateItemInRecoverableItems</span></span>](updateiteminrecoverableitems.md)
  
## <a name="text-value"></a><span data-ttu-id="5c857-114">Text value</span><span class="sxs-lookup"><span data-stu-id="5c857-114">Text value</span></span>

<span data-ttu-id="5c857-115">Um valor de texto de **true** para o elemento **MakeItemImmutable** indica que o item deve ser feito somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5c857-115">A text value of **true** for the **MakeItemImmutable** element indicates that the item should be made read-only.</span></span> <span data-ttu-id="5c857-116">Um valor **false** indica que o item permite o acesso de leitura / gravação.</span><span class="sxs-lookup"><span data-stu-id="5c857-116">A value of **false** indicates that the item allows read-write access.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5c857-117">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="5c857-117">Remarks</span></span>

<span data-ttu-id="5c857-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5c857-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5c857-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c857-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c857-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5c857-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c857-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="5c857-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5c857-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5c857-122">Schema name</span></span>  <br/> |<span data-ttu-id="5c857-123">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="5c857-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5c857-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5c857-124">Validation file</span></span>  <br/> |<span data-ttu-id="5c857-125">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5c857-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5c857-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="5c857-126">Can be empty</span></span>  <br/> ||
   

