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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824704"
---
# <a name="pendingmailtips"></a><span data-ttu-id="4fa90-103">PendingMailTips</span><span class="sxs-lookup"><span data-stu-id="4fa90-103">PendingMailTips</span></span>

<span data-ttu-id="4fa90-104">O elemento **PendingMailTips** indica que as dicas de email nesse elemento não pôde ser avaliadas antes de tempo limite de processamento do servidor expirou.</span><span class="sxs-lookup"><span data-stu-id="4fa90-104">The **PendingMailTips** element indicates that the mail tips in this element could not be evaluated before the server's processing timeout expired.</span></span> 
  
```XML
<PendingMailTips>All | OutOfOfficeMessage | MailboxFullStatus | CustomMailTip | ExternalMemberCount | TotalMemberCount | MaxMessageSize | DeliveryRestriction | ModerateStatus | InvalidRecipient</PendingMailTips>
```

 <span data-ttu-id="4fa90-105">**MailTipTypes**</span><span class="sxs-lookup"><span data-stu-id="4fa90-105">**MailTipTypes**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4fa90-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4fa90-106">Attributes and elements</span></span>

<span data-ttu-id="4fa90-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4fa90-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4fa90-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4fa90-108">Attributes</span></span>

<span data-ttu-id="4fa90-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4fa90-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4fa90-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4fa90-110">Child elements</span></span>

<span data-ttu-id="4fa90-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4fa90-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4fa90-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4fa90-112">Parent elements</span></span>

|<span data-ttu-id="4fa90-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4fa90-113">**Element**</span></span>|<span data-ttu-id="4fa90-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4fa90-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fa90-115">Dicas de email</span><span class="sxs-lookup"><span data-stu-id="4fa90-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="4fa90-116">Representa os valores para os vários tipos de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="4fa90-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4fa90-117">Text value</span><span class="sxs-lookup"><span data-stu-id="4fa90-117">Text value</span></span>

<span data-ttu-id="4fa90-118">A tabela a seguir lista os valores possíveis para o elemento **PendingMailTips** .</span><span class="sxs-lookup"><span data-stu-id="4fa90-118">The following table lists the possible values for the **PendingMailTips** element.</span></span> 
  
|<span data-ttu-id="4fa90-119">**Valor**</span><span class="sxs-lookup"><span data-stu-id="4fa90-119">**Value**</span></span>|<span data-ttu-id="4fa90-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4fa90-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4fa90-121">Todos</span><span class="sxs-lookup"><span data-stu-id="4fa90-121">All</span></span>  <br/> |<span data-ttu-id="4fa90-122">Representa todas as dicas de email disponíveis.</span><span class="sxs-lookup"><span data-stu-id="4fa90-122">Represents all available mail tips.</span></span>  <br/> |
|<span data-ttu-id="4fa90-123">OutOfOfficeMessage</span><span class="sxs-lookup"><span data-stu-id="4fa90-123">OutOfOfficeMessage</span></span>  <br/> |<span data-ttu-id="4fa90-124">Representa a mensagem de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="4fa90-124">Represents the Out of Office (OOF) message.</span></span>  <br/> |
|<span data-ttu-id="4fa90-125">MailboxFullStatus</span><span class="sxs-lookup"><span data-stu-id="4fa90-125">MailboxFullStatus</span></span>  <br/> |<span data-ttu-id="4fa90-126">Representa o status de uma caixa de correio que está sendo completo.</span><span class="sxs-lookup"><span data-stu-id="4fa90-126">Represents the status for a mailbox being full.</span></span>  <br/> |
|<span data-ttu-id="4fa90-127">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="4fa90-127">CustomMailTip</span></span>  <br/> |<span data-ttu-id="4fa90-128">Representa uma dica de email personalizado.</span><span class="sxs-lookup"><span data-stu-id="4fa90-128">Represents a custom mail tip.</span></span>  <br/> |
|<span data-ttu-id="4fa90-129">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="4fa90-129">ExternalMemberCount</span></span>  <br/> |<span data-ttu-id="4fa90-130">Representa a contagem de membros externos.</span><span class="sxs-lookup"><span data-stu-id="4fa90-130">Represents the count of external members.</span></span>  <br/> |
|<span data-ttu-id="4fa90-131">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="4fa90-131">TotalMemberCount</span></span>  <br/> |<span data-ttu-id="4fa90-132">Representa a contagem de todos os membros.</span><span class="sxs-lookup"><span data-stu-id="4fa90-132">Represents the count of all members.</span></span>  <br/> |
|<span data-ttu-id="4fa90-133">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="4fa90-133">MaxMessageSize</span></span>  <br/> |<span data-ttu-id="4fa90-134">Representa o tamanho de mensagem máximo que um destinatário pode aceitar.</span><span class="sxs-lookup"><span data-stu-id="4fa90-134">Represents the maximum message size a recipient can accept.</span></span>  <br/> |
|<span data-ttu-id="4fa90-135">DeliveryRestriction</span><span class="sxs-lookup"><span data-stu-id="4fa90-135">DeliveryRestriction</span></span>  <br/> |<span data-ttu-id="4fa90-136">Indica se as restrições de entrega impede que a mensagem do remetente está atingindo o destinatário.</span><span class="sxs-lookup"><span data-stu-id="4fa90-136">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|<span data-ttu-id="4fa90-137">ModerationStatus</span><span class="sxs-lookup"><span data-stu-id="4fa90-137">ModerationStatus</span></span>  <br/> |<span data-ttu-id="4fa90-138">Indica se a mensagem do remetente será revisada por um moderador.</span><span class="sxs-lookup"><span data-stu-id="4fa90-138">Indicates whether the sender's message will be reviewed by a moderator.</span></span>  <br/> |
|<span data-ttu-id="4fa90-139">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="4fa90-139">InvalidRecipient</span></span>  <br/> |<span data-ttu-id="4fa90-140">Indica se o destinatário é inválido.</span><span class="sxs-lookup"><span data-stu-id="4fa90-140">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4fa90-141">Comentários</span><span class="sxs-lookup"><span data-stu-id="4fa90-141">Remarks</span></span>

<span data-ttu-id="4fa90-142">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4fa90-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4fa90-143">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4fa90-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4fa90-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="4fa90-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4fa90-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4fa90-145">Schema Name</span></span>  <br/> |<span data-ttu-id="4fa90-146">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4fa90-146">Types schema</span></span>  <br/> |
|<span data-ttu-id="4fa90-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4fa90-147">Validation File</span></span>  <br/> |<span data-ttu-id="4fa90-148">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4fa90-148">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4fa90-149">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4fa90-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="4fa90-150">False</span><span class="sxs-lookup"><span data-stu-id="4fa90-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4fa90-151">Ver também</span><span class="sxs-lookup"><span data-stu-id="4fa90-151">See also</span></span>



- [<span data-ttu-id="4fa90-152">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4fa90-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

