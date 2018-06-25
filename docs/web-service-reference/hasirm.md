---
title: HasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fedc04e0-cfd2-4652-a2a8-51de859ae847
description: O elemento HasIrm Especifica se pelo menos uma mensagem na conversa e a pasta atual é uma mensagem protegida do IRM.
ms.openlocfilehash: c129370d7920da7cf1f9f32eed2f075e6c21cf8b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823803"
---
# <a name="hasirm"></a><span data-ttu-id="e2083-103">HasIrm</span><span class="sxs-lookup"><span data-stu-id="e2083-103">HasIrm</span></span>

<span data-ttu-id="e2083-104">O elemento **HasIrm** Especifica se pelo menos uma mensagem na conversa e a pasta atual é uma mensagem protegida do IRM.</span><span class="sxs-lookup"><span data-stu-id="e2083-104">The **HasIrm** element specifies whether at least one message in the conversation and the current folder is an IRM protected message.</span></span> 
  
```XML
<HasIrm> true | false </HasIrm>
```

 <span data-ttu-id="e2083-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e2083-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e2083-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e2083-106">Attributes and elements</span></span>

<span data-ttu-id="e2083-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e2083-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2083-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e2083-108">Attributes</span></span>

<span data-ttu-id="e2083-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e2083-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2083-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e2083-110">Child elements</span></span>

<span data-ttu-id="e2083-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e2083-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e2083-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e2083-112">Parent elements</span></span>

[<span data-ttu-id="e2083-113">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="e2083-113">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
## <a name="text-value"></a><span data-ttu-id="e2083-114">Text value</span><span class="sxs-lookup"><span data-stu-id="e2083-114">Text value</span></span>

<span data-ttu-id="e2083-115">O valor de texto do elemento **HasIrm** é **true** se pelo menos uma mensagem na conversa e a pasta atual tiver IRM.</span><span class="sxs-lookup"><span data-stu-id="e2083-115">The text value of the **HasIrm** element is **true** if at least one message in the conversation and the current folder has IRM.</span></span> <span data-ttu-id="e2083-116">Caso contrário, o valor é **false**.</span><span class="sxs-lookup"><span data-stu-id="e2083-116">Otherwise, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e2083-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="e2083-117">Remarks</span></span>

<span data-ttu-id="e2083-118">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e2083-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="e2083-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e2083-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e2083-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e2083-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2083-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="e2083-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e2083-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e2083-122">Schema Name</span></span>  <br/> |<span data-ttu-id="e2083-123">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e2083-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="e2083-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e2083-124">Validation File</span></span>  <br/> |<span data-ttu-id="e2083-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e2083-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e2083-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e2083-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="e2083-127">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="e2083-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e2083-128">Ver também</span><span class="sxs-lookup"><span data-stu-id="e2083-128">See also</span></span>



[<span data-ttu-id="e2083-129">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="e2083-129">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)


- [<span data-ttu-id="e2083-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e2083-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

