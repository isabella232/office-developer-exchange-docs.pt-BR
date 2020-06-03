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
description: O elemento Recipients representa uma coleção de destinatários que recebem uma cópia da mensagem.
ms.openlocfilehash: 0e18152a8143b888ad27f48137c06613694f5713
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463871"
---
# <a name="recipients-arrayofrecipientstype"></a><span data-ttu-id="bd333-103">Destinatários (ArrayOfRecipientsType)</span><span class="sxs-lookup"><span data-stu-id="bd333-103">Recipients (ArrayOfRecipientsType)</span></span>

<span data-ttu-id="bd333-104">O elemento **Recipients** representa uma coleção de destinatários que recebem uma cópia da mensagem.</span><span class="sxs-lookup"><span data-stu-id="bd333-104">The **Recipients** element represents a collection of recipients that receive a copy of the message.</span></span> 
  
```XML
<Recipients>
   <Mailbox/>
</Recipients>
```

 <span data-ttu-id="bd333-105">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="bd333-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd333-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="bd333-106">Attributes and elements</span></span>

<span data-ttu-id="bd333-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bd333-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd333-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="bd333-108">Attributes</span></span>

<span data-ttu-id="bd333-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bd333-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd333-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bd333-110">Child elements</span></span>

|<span data-ttu-id="bd333-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bd333-111">**Element**</span></span>|<span data-ttu-id="bd333-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bd333-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd333-113">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="bd333-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="bd333-114">Identifica um objeto do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="bd333-114">Identifies a mail-enabled Active Directory object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bd333-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bd333-115">Parent elements</span></span>

|<span data-ttu-id="bd333-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bd333-116">**Element**</span></span>|<span data-ttu-id="bd333-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bd333-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd333-118">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="bd333-118">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="bd333-119">Contém os destinatários e os tipos de dicas de email a serem recuperadas.</span><span class="sxs-lookup"><span data-stu-id="bd333-119">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bd333-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="bd333-120">Text value</span></span>

<span data-ttu-id="bd333-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bd333-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bd333-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="bd333-122">Remarks</span></span>

<span data-ttu-id="bd333-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd333-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd333-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="bd333-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd333-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="bd333-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bd333-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="bd333-126">Schema Name</span></span>  <br/> |<span data-ttu-id="bd333-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="bd333-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="bd333-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="bd333-128">Validation File</span></span>  <br/> |<span data-ttu-id="bd333-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bd333-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bd333-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="bd333-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="bd333-131">False</span><span class="sxs-lookup"><span data-stu-id="bd333-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bd333-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="bd333-132">See also</span></span>



- [<span data-ttu-id="bd333-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="bd333-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

