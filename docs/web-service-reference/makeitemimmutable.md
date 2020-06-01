---
title: MakeItemImmutable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: de1d2a60-aeeb-4625-8b11-23c42e1e7bae
description: O elemento MakeItemImmutable especifica um valor Boolean que indica se um item deve ser tornado somente leitura.
ms.openlocfilehash: 05c6e3343b8ba892048174ad98c9d31fe8da685b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465860"
---
# <a name="makeitemimmutable"></a><span data-ttu-id="55994-103">MakeItemImmutable</span><span class="sxs-lookup"><span data-stu-id="55994-103">MakeItemImmutable</span></span>

<span data-ttu-id="55994-104">O elemento **MakeItemImmutable** especifica um valor Boolean que indica se um item deve ser tornado somente leitura.</span><span class="sxs-lookup"><span data-stu-id="55994-104">The **MakeItemImmutable** element specifies a Boolean value that indicates whether an item should be made read-only.</span></span> 
  
```XML
<MakeItemImmutable>true | false</MakeItemImmutable>
```

 <span data-ttu-id="55994-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="55994-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55994-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="55994-106">Attributes and elements</span></span>

<span data-ttu-id="55994-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="55994-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55994-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="55994-108">Attributes</span></span>

<span data-ttu-id="55994-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55994-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55994-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="55994-110">Child elements</span></span>

<span data-ttu-id="55994-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="55994-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="55994-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="55994-112">Parent elements</span></span>

[<span data-ttu-id="55994-113">UpdateItemInRecoverableItems</span><span class="sxs-lookup"><span data-stu-id="55994-113">UpdateItemInRecoverableItems</span></span>](updateiteminrecoverableitems.md)
  
## <a name="text-value"></a><span data-ttu-id="55994-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="55994-114">Text value</span></span>

<span data-ttu-id="55994-115">Um valor de texto **true** para o elemento **MakeItemImmutable** indica que o item deve ser tornado somente leitura.</span><span class="sxs-lookup"><span data-stu-id="55994-115">A text value of **true** for the **MakeItemImmutable** element indicates that the item should be made read-only.</span></span> <span data-ttu-id="55994-116">Um valor **false** indica que o item permite acesso de leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="55994-116">A value of **false** indicates that the item allows read-write access.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="55994-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="55994-117">Remarks</span></span>

<span data-ttu-id="55994-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="55994-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="55994-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="55994-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55994-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="55994-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55994-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="55994-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="55994-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="55994-122">Schema name</span></span>  <br/> |<span data-ttu-id="55994-123">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="55994-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="55994-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="55994-124">Validation file</span></span>  <br/> |<span data-ttu-id="55994-125">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="55994-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="55994-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="55994-126">Can be empty</span></span>  <br/> ||
   

