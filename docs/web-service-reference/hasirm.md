---
title: HasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fedc04e0-cfd2-4652-a2a8-51de859ae847
description: O elemento HasIrm especifica se pelo menos uma mensagem na conversa e a pasta atual é uma mensagem protegida por IRM.
ms.openlocfilehash: 1596610ed5f6b2bac353900624fbec9140aaa693
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462777"
---
# <a name="hasirm"></a><span data-ttu-id="9729e-103">HasIrm</span><span class="sxs-lookup"><span data-stu-id="9729e-103">HasIrm</span></span>

<span data-ttu-id="9729e-104">O elemento **HasIrm** especifica se pelo menos uma mensagem na conversa e a pasta atual é uma mensagem protegida por IRM.</span><span class="sxs-lookup"><span data-stu-id="9729e-104">The **HasIrm** element specifies whether at least one message in the conversation and the current folder is an IRM protected message.</span></span> 
  
```XML
<HasIrm> true | false </HasIrm>
```

 <span data-ttu-id="9729e-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="9729e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9729e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9729e-106">Attributes and elements</span></span>

<span data-ttu-id="9729e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9729e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9729e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9729e-108">Attributes</span></span>

<span data-ttu-id="9729e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9729e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9729e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9729e-110">Child elements</span></span>

<span data-ttu-id="9729e-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9729e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9729e-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9729e-112">Parent elements</span></span>

[<span data-ttu-id="9729e-113">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="9729e-113">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
## <a name="text-value"></a><span data-ttu-id="9729e-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="9729e-114">Text value</span></span>

<span data-ttu-id="9729e-115">O valor de texto do elemento **HasIrm** é **true** se pelo menos uma mensagem na conversa e a pasta atual tem IRM.</span><span class="sxs-lookup"><span data-stu-id="9729e-115">The text value of the **HasIrm** element is **true** if at least one message in the conversation and the current folder has IRM.</span></span> <span data-ttu-id="9729e-116">Caso contrário, o valor será **false**.</span><span class="sxs-lookup"><span data-stu-id="9729e-116">Otherwise, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9729e-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="9729e-117">Remarks</span></span>

<span data-ttu-id="9729e-118">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9729e-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="9729e-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9729e-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9729e-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9729e-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9729e-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="9729e-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9729e-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9729e-122">Schema Name</span></span>  <br/> |<span data-ttu-id="9729e-123">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9729e-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="9729e-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9729e-124">Validation File</span></span>  <br/> |<span data-ttu-id="9729e-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9729e-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9729e-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9729e-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="9729e-127">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="9729e-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9729e-128">Confira também</span><span class="sxs-lookup"><span data-stu-id="9729e-128">See also</span></span>



[<span data-ttu-id="9729e-129">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="9729e-129">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)


- [<span data-ttu-id="9729e-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9729e-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

