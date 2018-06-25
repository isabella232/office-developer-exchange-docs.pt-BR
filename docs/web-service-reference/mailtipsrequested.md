---
title: MailTipsRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsRequested
api_type:
- schema
ms.assetid: 8037bbe5-a37f-4f77-8209-27a94f9095ef
description: O elemento MailTipsRequested contém os tipos de dicas de email solicitadas do serviço.
ms.openlocfilehash: fa2bef394ea8473aa65bdc2f1d39c0794186fdc6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824348"
---
# <a name="mailtipsrequested"></a><span data-ttu-id="b8d18-103">MailTipsRequested</span><span class="sxs-lookup"><span data-stu-id="b8d18-103">MailTipsRequested</span></span>

<span data-ttu-id="b8d18-104">O elemento **MailTipsRequested** contém os tipos de dicas de email solicitadas do serviço.</span><span class="sxs-lookup"><span data-stu-id="b8d18-104">The **MailTipsRequested** element contains the types of mail tips requested from the service.</span></span> 
  
```XML
<MailTipsRequested/>
```

 <span data-ttu-id="b8d18-105">**MailTipTypes**</span><span class="sxs-lookup"><span data-stu-id="b8d18-105">**MailTipTypes**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b8d18-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b8d18-106">Attributes and elements</span></span>

<span data-ttu-id="b8d18-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b8d18-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8d18-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b8d18-108">Attributes</span></span>

<span data-ttu-id="b8d18-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b8d18-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8d18-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b8d18-110">Child elements</span></span>

<span data-ttu-id="b8d18-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b8d18-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b8d18-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b8d18-112">Parent elements</span></span>

|<span data-ttu-id="b8d18-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b8d18-113">**Element**</span></span>|<span data-ttu-id="b8d18-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b8d18-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8d18-115">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="b8d18-115">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="b8d18-116">Contém os destinatários e os tipos de dicas de email para recuperar.</span><span class="sxs-lookup"><span data-stu-id="b8d18-116">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b8d18-117">Text value</span><span class="sxs-lookup"><span data-stu-id="b8d18-117">Text value</span></span>

<span data-ttu-id="b8d18-118">A tabela a seguir lista os valores possíveis para o elemento **MailTipsRequested** .</span><span class="sxs-lookup"><span data-stu-id="b8d18-118">The following table lists the possible values for the **MailTipsRequested** element.</span></span> 
  
|<span data-ttu-id="b8d18-119">**Valor**</span><span class="sxs-lookup"><span data-stu-id="b8d18-119">**Value**</span></span>|<span data-ttu-id="b8d18-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b8d18-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b8d18-121">Todos</span><span class="sxs-lookup"><span data-stu-id="b8d18-121">All</span></span>  <br/> |<span data-ttu-id="b8d18-122">Representa todas as dicas de email disponíveis.</span><span class="sxs-lookup"><span data-stu-id="b8d18-122">Represents all available mail tips.</span></span>  <br/> |
|<span data-ttu-id="b8d18-123">OutOfOfficeMessage</span><span class="sxs-lookup"><span data-stu-id="b8d18-123">OutOfOfficeMessage</span></span>  <br/> |<span data-ttu-id="b8d18-124">Representa a mensagem de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="b8d18-124">Represents the Out of Office (OOF) message.</span></span>  <br/> |
|<span data-ttu-id="b8d18-125">MailboxFullStatus</span><span class="sxs-lookup"><span data-stu-id="b8d18-125">MailboxFullStatus</span></span>  <br/> |<span data-ttu-id="b8d18-126">Representa o status de uma caixa de correio que está cheio.</span><span class="sxs-lookup"><span data-stu-id="b8d18-126">Represents the status for a mailbox that is full.</span></span>  <br/> |
|<span data-ttu-id="b8d18-127">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="b8d18-127">CustomMailTip</span></span>  <br/> |<span data-ttu-id="b8d18-128">Representa uma dica de email personalizado.</span><span class="sxs-lookup"><span data-stu-id="b8d18-128">Represents a custom mail tip.</span></span>  <br/> |
|<span data-ttu-id="b8d18-129">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="b8d18-129">ExternalMemberCount</span></span>  <br/> |<span data-ttu-id="b8d18-130">Representa a contagem de membros externos.</span><span class="sxs-lookup"><span data-stu-id="b8d18-130">Represents the count of external members.</span></span>  <br/> |
|<span data-ttu-id="b8d18-131">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="b8d18-131">TotalMemberCount</span></span>  <br/> |<span data-ttu-id="b8d18-132">Representa a contagem de todos os membros.</span><span class="sxs-lookup"><span data-stu-id="b8d18-132">Represents the count of all members.</span></span>  <br/> |
|<span data-ttu-id="b8d18-133">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="b8d18-133">MaxMessageSize</span></span>  <br/> |<span data-ttu-id="b8d18-134">Representa o tamanho de mensagem máximo que um destinatário pode aceitar.</span><span class="sxs-lookup"><span data-stu-id="b8d18-134">Represents the maximum message size a recipient can accept.</span></span>  <br/> |
|<span data-ttu-id="b8d18-135">DeliveryRestriction</span><span class="sxs-lookup"><span data-stu-id="b8d18-135">DeliveryRestriction</span></span>  <br/> |<span data-ttu-id="b8d18-136">Indica se as restrições de entrega impede que a mensagem do remetente está atingindo o destinatário.</span><span class="sxs-lookup"><span data-stu-id="b8d18-136">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|<span data-ttu-id="b8d18-137">ModerationStatus</span><span class="sxs-lookup"><span data-stu-id="b8d18-137">ModerationStatus</span></span>  <br/> |<span data-ttu-id="b8d18-138">Indica se a mensagem do remetente será revisada por um moderador.</span><span class="sxs-lookup"><span data-stu-id="b8d18-138">Indicates whether the sender's message will be reviewed by a moderator.</span></span>  <br/> |
|<span data-ttu-id="b8d18-139">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="b8d18-139">InvalidRecipient</span></span>  <br/> |<span data-ttu-id="b8d18-140">Indica se o destinatário é inválido.</span><span class="sxs-lookup"><span data-stu-id="b8d18-140">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b8d18-141">Comentários</span><span class="sxs-lookup"><span data-stu-id="b8d18-141">Remarks</span></span>

<span data-ttu-id="b8d18-142">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b8d18-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b8d18-143">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b8d18-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b8d18-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="b8d18-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b8d18-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b8d18-145">Schema Name</span></span>  <br/> |<span data-ttu-id="b8d18-146">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="b8d18-146">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b8d18-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b8d18-147">Validation File</span></span>  <br/> |<span data-ttu-id="b8d18-148">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b8d18-148">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b8d18-149">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b8d18-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="b8d18-150">False</span><span class="sxs-lookup"><span data-stu-id="b8d18-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b8d18-151">Ver também</span><span class="sxs-lookup"><span data-stu-id="b8d18-151">See also</span></span>



- [<span data-ttu-id="b8d18-152">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b8d18-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

