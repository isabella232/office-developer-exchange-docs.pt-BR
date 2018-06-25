---
title: Destinatários (ArrayOfRecipientsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recipients
api_type:
- schema
ms.assetid: f4b71403-cbae-4176-8b2e-3597048c057b
description: O elemento de destinatários representa uma coleção de destinatários que recebem uma cópia da mensagem.
ms.openlocfilehash: b24a029bfacd6cc40e85a201b8ca90efd7790e9f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824991"
---
# <a name="recipients-arrayofrecipientstype"></a><span data-ttu-id="d9e48-103">Destinatários (ArrayOfRecipientsType)</span><span class="sxs-lookup"><span data-stu-id="d9e48-103">Recipients (ArrayOfRecipientsType)</span></span>

<span data-ttu-id="d9e48-104">O elemento de **destinatários** representa uma coleção de destinatários que recebem uma cópia da mensagem.</span><span class="sxs-lookup"><span data-stu-id="d9e48-104">The **Recipients** element represents a collection of recipients that receive a copy of the message.</span></span> 
  
```XML
<Recipients>
   <Mailbox/>
</Recipients>
```

 <span data-ttu-id="d9e48-105">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="d9e48-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9e48-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d9e48-106">Attributes and elements</span></span>

<span data-ttu-id="d9e48-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d9e48-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9e48-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d9e48-108">Attributes</span></span>

<span data-ttu-id="d9e48-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d9e48-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9e48-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d9e48-110">Child elements</span></span>

|<span data-ttu-id="d9e48-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d9e48-111">**Element**</span></span>|<span data-ttu-id="d9e48-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d9e48-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9e48-113">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="d9e48-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="d9e48-114">Identifica um objeto do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="d9e48-114">Identifies a mail-enabled Active Directory object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d9e48-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d9e48-115">Parent elements</span></span>

|<span data-ttu-id="d9e48-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d9e48-116">**Element**</span></span>|<span data-ttu-id="d9e48-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d9e48-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9e48-118">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="d9e48-118">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="d9e48-119">Contém os destinatários e os tipos de dicas de email para recuperar.</span><span class="sxs-lookup"><span data-stu-id="d9e48-119">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d9e48-120">Text value</span><span class="sxs-lookup"><span data-stu-id="d9e48-120">Text value</span></span>

<span data-ttu-id="d9e48-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d9e48-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d9e48-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="d9e48-122">Remarks</span></span>

<span data-ttu-id="d9e48-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9e48-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9e48-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d9e48-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9e48-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="d9e48-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d9e48-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d9e48-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d9e48-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d9e48-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="d9e48-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d9e48-128">Validation File</span></span>  <br/> |<span data-ttu-id="d9e48-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d9e48-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d9e48-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d9e48-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d9e48-131">False</span><span class="sxs-lookup"><span data-stu-id="d9e48-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d9e48-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="d9e48-132">See also</span></span>



- [<span data-ttu-id="d9e48-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d9e48-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

