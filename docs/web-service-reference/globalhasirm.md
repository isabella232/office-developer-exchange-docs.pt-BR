---
title: GlobalHasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 425272b2-7a4e-4376-aea9-d9b10c1ad6ee
description: O elemento GlobalHasIrm especifica se pelo menos uma mensagem na conversa e em todas as pastas é uma mensagem protegida por IRM.
ms.openlocfilehash: 10b99c9a6421a89a549b69e918087f3e542ffa09
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459466"
---
# <a name="globalhasirm"></a><span data-ttu-id="a0ffb-103">GlobalHasIrm</span><span class="sxs-lookup"><span data-stu-id="a0ffb-103">GlobalHasIrm</span></span>

<span data-ttu-id="a0ffb-104">O elemento **GlobalHasIrm** especifica se pelo menos uma mensagem na conversa e em todas as pastas é uma mensagem protegida por IRM.</span><span class="sxs-lookup"><span data-stu-id="a0ffb-104">The **GlobalHasIrm** element specifies whether at least one message in the conversation and across all folders is an IRM protected message.</span></span> 
  
```XML
<GlobalHasIrm> true | false </GlobalHasIrm>
```

 <span data-ttu-id="a0ffb-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a0ffb-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0ffb-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a0ffb-106">Attributes and elements</span></span>

<span data-ttu-id="a0ffb-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a0ffb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0ffb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a0ffb-108">Attributes</span></span>

<span data-ttu-id="a0ffb-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a0ffb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a0ffb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a0ffb-110">Child elements</span></span>

<span data-ttu-id="a0ffb-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a0ffb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a0ffb-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a0ffb-112">Parent elements</span></span>

[<span data-ttu-id="a0ffb-113">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="a0ffb-113">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
## <a name="text-value"></a><span data-ttu-id="a0ffb-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a0ffb-114">Text value</span></span>

<span data-ttu-id="a0ffb-115">O valor de texto do elemento **GlobalHasIrm** será **true** se pelo menos uma mensagem na conversa e em todas as pastas for uma mensagem protegida por IRM.</span><span class="sxs-lookup"><span data-stu-id="a0ffb-115">The text value of the **GlobalHasIrm** element is **true** if at least one message in the conversation and across all folders is an IRM protected message.</span></span> <span data-ttu-id="a0ffb-116">Caso contrário, o valor será **false**.</span><span class="sxs-lookup"><span data-stu-id="a0ffb-116">Otherwise the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a0ffb-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="a0ffb-117">Remarks</span></span>

<span data-ttu-id="a0ffb-118">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a0ffb-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="a0ffb-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0ffb-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a0ffb-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a0ffb-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0ffb-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="a0ffb-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a0ffb-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a0ffb-122">Schema Name</span></span>  <br/> |<span data-ttu-id="a0ffb-123">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a0ffb-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="a0ffb-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a0ffb-124">Validation File</span></span>  <br/> |<span data-ttu-id="a0ffb-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a0ffb-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a0ffb-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a0ffb-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="a0ffb-127">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="a0ffb-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a0ffb-128">Também consulte</span><span class="sxs-lookup"><span data-stu-id="a0ffb-128">See also</span></span>



[<span data-ttu-id="a0ffb-129">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="a0ffb-129">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)


- [<span data-ttu-id="a0ffb-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a0ffb-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

