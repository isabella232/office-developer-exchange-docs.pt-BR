---
title: Guid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 49dcf69f-bf8d-4be6-a24c-03bbd13f4fe5
description: O elemento GUID especifica o identificador global exclusivo da caixa de correio.
ms.openlocfilehash: 4db66b5ae2c67f64f75c69a3d77cfa2b587775be
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530772"
---
# <a name="guid"></a><span data-ttu-id="17518-103">Guid</span><span class="sxs-lookup"><span data-stu-id="17518-103">Guid</span></span>

<span data-ttu-id="17518-104">O elemento **GUID** especifica o identificador global exclusivo da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="17518-104">The **Guid** element specifies the globally unique identifier of the mailbox.</span></span> 
  
```XML
<Guid></Guid>
```

 <span data-ttu-id="17518-105">**Guidtype**</span><span class="sxs-lookup"><span data-stu-id="17518-105">**GuidType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="17518-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="17518-106">Attributes and elements</span></span>

<span data-ttu-id="17518-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="17518-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="17518-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="17518-108">Attributes</span></span>

<span data-ttu-id="17518-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="17518-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="17518-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="17518-110">Child elements</span></span>

<span data-ttu-id="17518-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="17518-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="17518-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="17518-112">Parent elements</span></span>

|<span data-ttu-id="17518-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="17518-113">**Element**</span></span>|<span data-ttu-id="17518-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="17518-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17518-115">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="17518-115">SearchableMailbox</span></span>](searchablemailbox.md) <br/> |<span data-ttu-id="17518-116">Especifica uma caixa de correio retornada de uma solicitação **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="17518-116">Specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="17518-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="17518-117">Text value</span></span>

<span data-ttu-id="17518-118">O valor de texto do elemento **GUID** é um valor de GUID que identifica exclusivamente uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="17518-118">The text value of the **Guid** element is a GUID value that uniquely identifies a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="17518-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="17518-119">Remarks</span></span>

<span data-ttu-id="17518-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="17518-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="17518-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="17518-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="17518-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="17518-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="17518-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="17518-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="17518-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="17518-124">Schema Name</span></span>  <br/> |<span data-ttu-id="17518-125">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="17518-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="17518-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="17518-126">Validation File</span></span>  <br/> |<span data-ttu-id="17518-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="17518-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="17518-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="17518-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="17518-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="17518-129">See also</span></span>



- [<span data-ttu-id="17518-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="17518-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

