---
title: Dicas de email
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTips
api_type:
- schema
ms.assetid: c1cba493-bccc-4b8e-be8e-bfa8a8b10882
description: O elemento de dicas de email representa os valores para os vários tipos de dicas de email.
ms.openlocfilehash: 3a2e95225b09fd2d81db32f821ea3069ab7e7852
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824311"
---
# <a name="mailtips"></a><span data-ttu-id="2d8f7-103">Dicas de email</span><span class="sxs-lookup"><span data-stu-id="2d8f7-103">MailTips</span></span>

<span data-ttu-id="2d8f7-104">O elemento de **dicas de email** representa os valores para os vários tipos de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="2d8f7-104">The **MailTips** element represents values for various types of mail tips.</span></span> 
  
```XML
<MailTips>
   <RecipientAddress/>
   <PendingMailTips/>
   <OutOfOffice/>
   <MailboxFull/>
   <CustomMailTip/>
   <TotalMemberCount/>
   <ExternalMemberCount/>
   <MaxMessageSize/>
   <DeliveryRestricted/>
   <IsModerated/>
   <InvalidRecipient/>
</MailTips>
```

 <span data-ttu-id="2d8f7-105">**Dicas de email**</span><span class="sxs-lookup"><span data-stu-id="2d8f7-105">**MailTips**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2d8f7-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2d8f7-106">Attributes and elements</span></span>

<span data-ttu-id="2d8f7-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2d8f7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d8f7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2d8f7-108">Attributes</span></span>

<span data-ttu-id="2d8f7-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2d8f7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d8f7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2d8f7-110">Child elements</span></span>

|<span data-ttu-id="2d8f7-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2d8f7-111">**Element**</span></span>|<span data-ttu-id="2d8f7-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2d8f7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d8f7-113">RecipientAddress</span><span class="sxs-lookup"><span data-stu-id="2d8f7-113">RecipientAddress</span></span>](recipientaddress.md) <br/> |<span data-ttu-id="2d8f7-114">Representa a caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="2d8f7-114">Represents the mailbox of the recipient.</span></span>  <br/> |
|[<span data-ttu-id="2d8f7-115">PendingMailTips</span><span class="sxs-lookup"><span data-stu-id="2d8f7-115">PendingMailTips</span></span>](pendingmailtips.md) <br/> |<span data-ttu-id="2d8f7-116">Indica que as dicas de email nesse elemento não pôde ser avaliadas antes de tempo limite de processamento do servidor expirou.</span><span class="sxs-lookup"><span data-stu-id="2d8f7-116">Indicates that the mail tips in this element could not be evaluated before the server's processing timeout expired.</span></span>  <br/> |
|[<span data-ttu-id="2d8f7-117">Fora do escritório</span><span class="sxs-lookup"><span data-stu-id="2d8f7-117">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="2d8f7-118">Representa a mensagem de resposta e um tempo de duração para enviar a mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="2d8f7-118">Represents the response message and a duration time for sending the response message.</span></span>  <br/> |
|[<span data-ttu-id="2d8f7-119">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="2d8f7-119">MailboxFull</span></span>](mailboxfull.md) <br/> |<span data-ttu-id="2d8f7-120">Indica se a caixa de correio do destinatário está cheio.</span><span class="sxs-lookup"><span data-stu-id="2d8f7-120">Indicates whether the mailbox for the recipient is full.</span></span>  <br/> |
|[<span data-ttu-id="2d8f7-121">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="2d8f7-121">CustomMailTip</span></span>](custommailtip.md) <br/> |<span data-ttu-id="2d8f7-122">Representa uma mensagem de dica de email personalizada.</span><span class="sxs-lookup"><span data-stu-id="2d8f7-122">Represents a customized mail tip message.</span></span>  <br/> |
|[<span data-ttu-id="2d8f7-123">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="2d8f7-123">TotalMemberCount</span></span>](totalmembercount.md) <br/> |<span data-ttu-id="2d8f7-124">Representa a contagem de todos os membros em um grupo.</span><span class="sxs-lookup"><span data-stu-id="2d8f7-124">Represents the count of all members in a group.</span></span>  <br/> |
|[<span data-ttu-id="2d8f7-125">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="2d8f7-125">ExternalMemberCount</span></span>](externalmembercount.md) <br/> |<span data-ttu-id="2d8f7-126">Representa a contagem de membros externos em um grupo.</span><span class="sxs-lookup"><span data-stu-id="2d8f7-126">Represents the count of external members in a group.</span></span>  <br/> |
|[<span data-ttu-id="2d8f7-127">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="2d8f7-127">MaxMessageSize</span></span>](maxmessagesize.md) <br/> |<span data-ttu-id="2d8f7-128">Representa o tamanho máximo da mensagem que o destinatário possa aceitar.</span><span class="sxs-lookup"><span data-stu-id="2d8f7-128">Represents the maximum message size the recipient can accept.</span></span>  <br/> |
|[<span data-ttu-id="2d8f7-129">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="2d8f7-129">DeliveryRestricted</span></span>](deliveryrestricted.md) <br/> |<span data-ttu-id="2d8f7-130">Indica se as restrições de entrega impede que a mensagem do remetente está atingindo o destinatário.</span><span class="sxs-lookup"><span data-stu-id="2d8f7-130">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|[<span data-ttu-id="2d8f7-131">IsModerated</span><span class="sxs-lookup"><span data-stu-id="2d8f7-131">IsModerated</span></span>](ismoderated.md) <br/> |<span data-ttu-id="2d8f7-132">Indica se a caixa de correio do destinatário está sendo moderada.</span><span class="sxs-lookup"><span data-stu-id="2d8f7-132">Indicates whether the recipient's mailbox is being moderated.</span></span>  <br/> |
|[<span data-ttu-id="2d8f7-133">InvalidRecipient (dicas de email)</span><span class="sxs-lookup"><span data-stu-id="2d8f7-133">InvalidRecipient (MailTips)</span></span>](invalidrecipient-mailtips.md) <br/> |<span data-ttu-id="2d8f7-134">Indica se o destinatário é inválido.</span><span class="sxs-lookup"><span data-stu-id="2d8f7-134">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2d8f7-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2d8f7-135">Parent elements</span></span>

|<span data-ttu-id="2d8f7-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2d8f7-136">**Element**</span></span>|<span data-ttu-id="2d8f7-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2d8f7-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d8f7-138">MailTipsResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="2d8f7-138">MailTipsResponseMessageType</span></span>](mailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="2d8f7-139">Representa as configurações de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="2d8f7-139">Represents mail tips settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2d8f7-140">Text value</span><span class="sxs-lookup"><span data-stu-id="2d8f7-140">Text value</span></span>

<span data-ttu-id="2d8f7-141">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2d8f7-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2d8f7-142">Comentários</span><span class="sxs-lookup"><span data-stu-id="2d8f7-142">Remarks</span></span>

<span data-ttu-id="2d8f7-143">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d8f7-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2d8f7-144">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2d8f7-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2d8f7-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="2d8f7-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2d8f7-146">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2d8f7-146">Schema Name</span></span>  <br/> |<span data-ttu-id="2d8f7-147">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="2d8f7-147">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2d8f7-148">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2d8f7-148">Validation File</span></span>  <br/> |<span data-ttu-id="2d8f7-149">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2d8f7-149">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2d8f7-150">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2d8f7-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="2d8f7-151">False</span><span class="sxs-lookup"><span data-stu-id="2d8f7-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2d8f7-152">Ver também</span><span class="sxs-lookup"><span data-stu-id="2d8f7-152">See also</span></span>



- [<span data-ttu-id="2d8f7-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2d8f7-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

