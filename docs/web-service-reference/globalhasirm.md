---
title: GlobalHasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 425272b2-7a4e-4376-aea9-d9b10c1ad6ee
description: O elemento GlobalHasIrm Especifica se pelo menos uma mensagem na conversa e em todas as pastas é uma mensagem protegida do IRM.
ms.openlocfilehash: ad3eafcb38829e7ea57cbc7535b0f5411ad595d2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823717"
---
# <a name="globalhasirm"></a><span data-ttu-id="57d82-103">GlobalHasIrm</span><span class="sxs-lookup"><span data-stu-id="57d82-103">GlobalHasIrm</span></span>

<span data-ttu-id="57d82-104">O elemento **GlobalHasIrm** Especifica se pelo menos uma mensagem na conversa e em todas as pastas é uma mensagem protegida do IRM.</span><span class="sxs-lookup"><span data-stu-id="57d82-104">The **GlobalHasIrm** element specifies whether at least one message in the conversation and across all folders is an IRM protected message.</span></span> 
  
```XML
<GlobalHasIrm> true | false </GlobalHasIrm>
```

 <span data-ttu-id="57d82-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="57d82-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57d82-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="57d82-106">Attributes and elements</span></span>

<span data-ttu-id="57d82-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="57d82-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57d82-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="57d82-108">Attributes</span></span>

<span data-ttu-id="57d82-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="57d82-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57d82-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="57d82-110">Child elements</span></span>

<span data-ttu-id="57d82-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="57d82-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="57d82-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="57d82-112">Parent elements</span></span>

[<span data-ttu-id="57d82-113">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="57d82-113">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
## <a name="text-value"></a><span data-ttu-id="57d82-114">Text value</span><span class="sxs-lookup"><span data-stu-id="57d82-114">Text value</span></span>

<span data-ttu-id="57d82-115">O valor de texto do elemento **GlobalHasIrm** é **true** se pelo menos uma mensagem na conversa e em todas as pastas é uma mensagem protegida do IRM.</span><span class="sxs-lookup"><span data-stu-id="57d82-115">The text value of the **GlobalHasIrm** element is **true** if at least one message in the conversation and across all folders is an IRM protected message.</span></span> <span data-ttu-id="57d82-116">Caso contrário, o valor é **false**.</span><span class="sxs-lookup"><span data-stu-id="57d82-116">Otherwise the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="57d82-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="57d82-117">Remarks</span></span>

<span data-ttu-id="57d82-118">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="57d82-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="57d82-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="57d82-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57d82-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="57d82-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57d82-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="57d82-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="57d82-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="57d82-122">Schema Name</span></span>  <br/> |<span data-ttu-id="57d82-123">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="57d82-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="57d82-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="57d82-124">Validation File</span></span>  <br/> |<span data-ttu-id="57d82-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="57d82-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="57d82-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="57d82-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="57d82-127">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="57d82-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57d82-128">Ver também</span><span class="sxs-lookup"><span data-stu-id="57d82-128">See also</span></span>



[<span data-ttu-id="57d82-129">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="57d82-129">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)


- [<span data-ttu-id="57d82-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="57d82-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

