---
title: ErrorCode (int)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 65537d96-edf9-41ee-9ad5-91ffe37e2269
description: O elemento ErrorCode Especifica o código de erro de uma pesquisa com falha realizada em uma caixa de correio.
ms.openlocfilehash: ed8a7771376f921303ea093f4be727c4146faa76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752087"
---
# <a name="errorcode-int"></a><span data-ttu-id="ea7f7-103">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="ea7f7-103">ErrorCode (int)</span></span>

<span data-ttu-id="ea7f7-104">O elemento **ErrorCode** Especifica o código de erro de uma pesquisa com falha realizada em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ea7f7-104">The **ErrorCode** element specifies the error code of a failed search performed against a mailbox.</span></span> 
  
```XML
<ErrorCode></ErrorCode>
```

 <span data-ttu-id="ea7f7-105">**int**</span><span class="sxs-lookup"><span data-stu-id="ea7f7-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ea7f7-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ea7f7-106">Attributes and elements</span></span>

<span data-ttu-id="ea7f7-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ea7f7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea7f7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ea7f7-108">Attributes</span></span>

<span data-ttu-id="ea7f7-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ea7f7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ea7f7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ea7f7-110">Child elements</span></span>

<span data-ttu-id="ea7f7-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ea7f7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ea7f7-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ea7f7-112">Parent elements</span></span>

|<span data-ttu-id="ea7f7-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ea7f7-113">**Element**</span></span>|<span data-ttu-id="ea7f7-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ea7f7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea7f7-115">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="ea7f7-115">FailedMailbox</span></span>](failedmailbox.md) <br/> |<span data-ttu-id="ea7f7-116">Especifica o status de retenção da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ea7f7-116">Specifies the hold status of the mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ea7f7-117">Text value</span><span class="sxs-lookup"><span data-stu-id="ea7f7-117">Text value</span></span>

<span data-ttu-id="ea7f7-118">O valor de texto do elemento **ErrorCode** é o código de erro retornado para uma pesquisa com falha realizada em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ea7f7-118">The text value of the **ErrorCode** element is the error code returned for a failed search performed against a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ea7f7-119">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="ea7f7-119">Remarks</span></span>

<span data-ttu-id="ea7f7-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ea7f7-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ea7f7-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ea7f7-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ea7f7-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ea7f7-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea7f7-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="ea7f7-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ea7f7-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ea7f7-124">Schema Name</span></span>  <br/> |<span data-ttu-id="ea7f7-125">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="ea7f7-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="ea7f7-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ea7f7-126">Validation File</span></span>  <br/> |<span data-ttu-id="ea7f7-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ea7f7-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="ea7f7-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ea7f7-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ea7f7-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="ea7f7-129">See also</span></span>



- [<span data-ttu-id="ea7f7-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ea7f7-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

