---
title: ErrorCode (int)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 65537d96-edf9-41ee-9ad5-91ffe37e2269
description: O elemento ErrorCode especifica o código de erro de uma pesquisa com falha realizada em relação a uma caixa de correio.
ms.openlocfilehash: 24170a56e5fa23c3811fcbd27f0240e6ba3c87b7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460663"
---
# <a name="errorcode-int"></a><span data-ttu-id="925a2-103">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="925a2-103">ErrorCode (int)</span></span>

<span data-ttu-id="925a2-104">O elemento **ErrorCode** especifica o código de erro de uma pesquisa com falha realizada em relação a uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="925a2-104">The **ErrorCode** element specifies the error code of a failed search performed against a mailbox.</span></span> 
  
```XML
<ErrorCode></ErrorCode>
```

 <span data-ttu-id="925a2-105">**int**</span><span class="sxs-lookup"><span data-stu-id="925a2-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="925a2-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="925a2-106">Attributes and elements</span></span>

<span data-ttu-id="925a2-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="925a2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="925a2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="925a2-108">Attributes</span></span>

<span data-ttu-id="925a2-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="925a2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="925a2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="925a2-110">Child elements</span></span>

<span data-ttu-id="925a2-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="925a2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="925a2-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="925a2-112">Parent elements</span></span>

|<span data-ttu-id="925a2-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="925a2-113">**Element**</span></span>|<span data-ttu-id="925a2-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="925a2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="925a2-115">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="925a2-115">FailedMailbox</span></span>](failedmailbox.md) <br/> |<span data-ttu-id="925a2-116">Especifica o status de retenção da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="925a2-116">Specifies the hold status of the mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="925a2-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="925a2-117">Text value</span></span>

<span data-ttu-id="925a2-118">O valor de texto do elemento **ErrorCode** é o código de erro retornado para uma pesquisa com falha realizada em relação a uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="925a2-118">The text value of the **ErrorCode** element is the error code returned for a failed search performed against a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="925a2-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="925a2-119">Remarks</span></span>

<span data-ttu-id="925a2-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="925a2-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="925a2-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="925a2-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="925a2-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="925a2-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="925a2-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="925a2-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="925a2-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="925a2-124">Schema Name</span></span>  <br/> |<span data-ttu-id="925a2-125">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="925a2-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="925a2-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="925a2-126">Validation File</span></span>  <br/> |<span data-ttu-id="925a2-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="925a2-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="925a2-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="925a2-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="925a2-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="925a2-129">See also</span></span>



- [<span data-ttu-id="925a2-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="925a2-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

