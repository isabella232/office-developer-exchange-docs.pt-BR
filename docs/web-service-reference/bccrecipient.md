---
title: BccRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BccRecipient
api_type:
- schema
ms.assetid: 4ef0cff5-8a5a-4d76-9d2b-938774d8fc1b
description: O elemento BccRecipient representa um destinatário para receber uma cópia oculta (Cco) de uma mensagem de email.
ms.openlocfilehash: 8296af1d74338bdfb1f4cb7bc7449ad91a9cd531
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461524"
---
# <a name="bccrecipient"></a><span data-ttu-id="0e790-103">BccRecipient</span><span class="sxs-lookup"><span data-stu-id="0e790-103">BccRecipient</span></span>

<span data-ttu-id="0e790-104">O elemento **BccRecipient** representa um destinatário para receber uma cópia oculta (Cco) de uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="0e790-104">The **BccRecipient** element represents a recipient to receive a blind carbon copy (Bcc) of an e-mail message.</span></span> 
  
```XML
<BccRecipient>true | false</BccRecipient>
```

 <span data-ttu-id="0e790-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="0e790-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0e790-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0e790-106">Attributes and elements</span></span>

<span data-ttu-id="0e790-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0e790-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e790-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0e790-108">Attributes</span></span>

<span data-ttu-id="0e790-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0e790-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e790-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0e790-110">Child elements</span></span>

<span data-ttu-id="0e790-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0e790-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0e790-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0e790-112">Parent elements</span></span>

|<span data-ttu-id="0e790-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0e790-113">**Element**</span></span>|<span data-ttu-id="0e790-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0e790-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e790-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="0e790-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="0e790-116">Contém informações de um único evento para um destinatário.</span><span class="sxs-lookup"><span data-stu-id="0e790-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0e790-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="0e790-117">Text value</span></span>

<span data-ttu-id="0e790-118">Esse elemento pode ser **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="0e790-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="0e790-119">Um valor **true** indica que o destinatário é com cópia oculta; um valor **false** indica que o destinatário não está com cópia oculta.</span><span class="sxs-lookup"><span data-stu-id="0e790-119">A value of **true** indicates that the recipient is blind carbon copied; a value of **false** indicates that the recipient is not blind carbon copied.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0e790-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="0e790-120">Remarks</span></span>

<span data-ttu-id="0e790-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0e790-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0e790-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0e790-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e790-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="0e790-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0e790-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0e790-124">Schema Name</span></span>  <br/> |<span data-ttu-id="0e790-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0e790-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="0e790-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0e790-126">Validation File</span></span>  <br/> |<span data-ttu-id="0e790-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0e790-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0e790-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0e790-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="0e790-129">False</span><span class="sxs-lookup"><span data-stu-id="0e790-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0e790-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="0e790-130">See also</span></span>



- [<span data-ttu-id="0e790-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0e790-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

