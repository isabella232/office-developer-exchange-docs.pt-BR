---
title: PendingMailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PendingMailTips
api_type:
- schema
ms.assetid: 0cd70eea-8d36-4b1b-bf80-5edf359e7ba7
description: O elemento PendingMailTips indica que as dicas de email nesse elemento não pôde ser avaliadas antes de tempo limite de processamento do servidor expirou.
ms.openlocfilehash: 73d597f6534ea29f7d26d6526c48631251521ae5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824704"
---
# <a name="pendingmailtips"></a><span data-ttu-id="9edf8-103">PendingMailTips</span><span class="sxs-lookup"><span data-stu-id="9edf8-103">PendingMailTips</span></span>

<span data-ttu-id="9edf8-104">O elemento **PendingMailTips** indica que as dicas de email nesse elemento não pôde ser avaliadas antes de tempo limite de processamento do servidor expirou.</span><span class="sxs-lookup"><span data-stu-id="9edf8-104">The **PendingMailTips** element indicates that the mail tips in this element could not be evaluated before the server's processing timeout expired.</span></span> 
  
```XML
<PendingMailTips>All | OutOfOfficeMessage | MailboxFullStatus | CustomMailTip | ExternalMemberCount | TotalMemberCount | MaxMessageSize | DeliveryRestriction | ModerateStatus | InvalidRecipient</PendingMailTips>
```

 <span data-ttu-id="9edf8-105">**MailTipTypes**</span><span class="sxs-lookup"><span data-stu-id="9edf8-105">**MailTipTypes**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9edf8-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9edf8-106">Attributes and elements</span></span>

<span data-ttu-id="9edf8-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9edf8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9edf8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9edf8-108">Attributes</span></span>

<span data-ttu-id="9edf8-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9edf8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9edf8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9edf8-110">Child elements</span></span>

<span data-ttu-id="9edf8-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9edf8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9edf8-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9edf8-112">Parent elements</span></span>

|<span data-ttu-id="9edf8-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9edf8-113">**Element**</span></span>|<span data-ttu-id="9edf8-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9edf8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9edf8-115">Dicas de email</span><span class="sxs-lookup"><span data-stu-id="9edf8-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="9edf8-116">Representa os valores para os vários tipos de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="9edf8-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9edf8-117">Text value</span><span class="sxs-lookup"><span data-stu-id="9edf8-117">Text value</span></span>

<span data-ttu-id="9edf8-118">A tabela a seguir lista os valores possíveis para o elemento **PendingMailTips** .</span><span class="sxs-lookup"><span data-stu-id="9edf8-118">The following table lists the possible values for the **PendingMailTips** element.</span></span> 
  
|<span data-ttu-id="9edf8-119">**Valor**</span><span class="sxs-lookup"><span data-stu-id="9edf8-119">**Value**</span></span>|<span data-ttu-id="9edf8-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9edf8-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9edf8-121">Todos</span><span class="sxs-lookup"><span data-stu-id="9edf8-121">All</span></span>  <br/> |<span data-ttu-id="9edf8-122">Representa todas as dicas de email disponíveis.</span><span class="sxs-lookup"><span data-stu-id="9edf8-122">Represents all available mail tips.</span></span>  <br/> |
|<span data-ttu-id="9edf8-123">OutOfOfficeMessage</span><span class="sxs-lookup"><span data-stu-id="9edf8-123">OutOfOfficeMessage</span></span>  <br/> |<span data-ttu-id="9edf8-124">Representa a mensagem de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="9edf8-124">Represents the Out of Office (OOF) message.</span></span>  <br/> |
|<span data-ttu-id="9edf8-125">MailboxFullStatus</span><span class="sxs-lookup"><span data-stu-id="9edf8-125">MailboxFullStatus</span></span>  <br/> |<span data-ttu-id="9edf8-126">Representa o status de uma caixa de correio que está sendo completo.</span><span class="sxs-lookup"><span data-stu-id="9edf8-126">Represents the status for a mailbox being full.</span></span>  <br/> |
|<span data-ttu-id="9edf8-127">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="9edf8-127">CustomMailTip</span></span>  <br/> |<span data-ttu-id="9edf8-128">Representa uma dica de email personalizado.</span><span class="sxs-lookup"><span data-stu-id="9edf8-128">Represents a custom mail tip.</span></span>  <br/> |
|<span data-ttu-id="9edf8-129">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="9edf8-129">ExternalMemberCount</span></span>  <br/> |<span data-ttu-id="9edf8-130">Representa a contagem de membros externos.</span><span class="sxs-lookup"><span data-stu-id="9edf8-130">Represents the count of external members.</span></span>  <br/> |
|<span data-ttu-id="9edf8-131">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="9edf8-131">TotalMemberCount</span></span>  <br/> |<span data-ttu-id="9edf8-132">Representa a contagem de todos os membros.</span><span class="sxs-lookup"><span data-stu-id="9edf8-132">Represents the count of all members.</span></span>  <br/> |
|<span data-ttu-id="9edf8-133">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="9edf8-133">MaxMessageSize</span></span>  <br/> |<span data-ttu-id="9edf8-134">Representa o tamanho de mensagem máximo que um destinatário pode aceitar.</span><span class="sxs-lookup"><span data-stu-id="9edf8-134">Represents the maximum message size a recipient can accept.</span></span>  <br/> |
|<span data-ttu-id="9edf8-135">DeliveryRestriction</span><span class="sxs-lookup"><span data-stu-id="9edf8-135">DeliveryRestriction</span></span>  <br/> |<span data-ttu-id="9edf8-136">Indica se as restrições de entrega impede que a mensagem do remetente está atingindo o destinatário.</span><span class="sxs-lookup"><span data-stu-id="9edf8-136">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|<span data-ttu-id="9edf8-137">ModerationStatus</span><span class="sxs-lookup"><span data-stu-id="9edf8-137">ModerationStatus</span></span>  <br/> |<span data-ttu-id="9edf8-138">Indica se a mensagem do remetente será revisada por um moderador.</span><span class="sxs-lookup"><span data-stu-id="9edf8-138">Indicates whether the sender's message will be reviewed by a moderator.</span></span>  <br/> |
|<span data-ttu-id="9edf8-139">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="9edf8-139">InvalidRecipient</span></span>  <br/> |<span data-ttu-id="9edf8-140">Indica se o destinatário é inválido.</span><span class="sxs-lookup"><span data-stu-id="9edf8-140">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9edf8-141">Comentários</span><span class="sxs-lookup"><span data-stu-id="9edf8-141">Remarks</span></span>

<span data-ttu-id="9edf8-142">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9edf8-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9edf8-143">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9edf8-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9edf8-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="9edf8-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9edf8-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9edf8-145">Schema Name</span></span>  <br/> |<span data-ttu-id="9edf8-146">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9edf8-146">Types schema</span></span>  <br/> |
|<span data-ttu-id="9edf8-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9edf8-147">Validation File</span></span>  <br/> |<span data-ttu-id="9edf8-148">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9edf8-148">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9edf8-149">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9edf8-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="9edf8-150">False</span><span class="sxs-lookup"><span data-stu-id="9edf8-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9edf8-151">Ver também</span><span class="sxs-lookup"><span data-stu-id="9edf8-151">See also</span></span>



- [<span data-ttu-id="9edf8-152">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9edf8-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

