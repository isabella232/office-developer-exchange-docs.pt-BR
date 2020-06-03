---
title: MailTips
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
description: O elemento de dicas de email representa valores de vários tipos de dicas de email.
ms.openlocfilehash: 9bacdea7b4f3108f700ed102025445e01a73e69d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44447593"
---
# <a name="mailtips"></a><span data-ttu-id="208a3-103">MailTips</span><span class="sxs-lookup"><span data-stu-id="208a3-103">MailTips</span></span>

<span data-ttu-id="208a3-104">O elemento de **dicas** de email representa valores de vários tipos de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="208a3-104">The **MailTips** element represents values for various types of mail tips.</span></span> 
  
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

 <span data-ttu-id="208a3-105">**Dicas de Email**</span><span class="sxs-lookup"><span data-stu-id="208a3-105">**MailTips**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="208a3-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="208a3-106">Attributes and elements</span></span>

<span data-ttu-id="208a3-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="208a3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="208a3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="208a3-108">Attributes</span></span>

<span data-ttu-id="208a3-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="208a3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="208a3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="208a3-110">Child elements</span></span>

|<span data-ttu-id="208a3-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="208a3-111">**Element**</span></span>|<span data-ttu-id="208a3-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="208a3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="208a3-113">RecipientAddress</span><span class="sxs-lookup"><span data-stu-id="208a3-113">RecipientAddress</span></span>](recipientaddress.md) <br/> |<span data-ttu-id="208a3-114">Representa a caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="208a3-114">Represents the mailbox of the recipient.</span></span>  <br/> |
|[<span data-ttu-id="208a3-115">PendingMailTips</span><span class="sxs-lookup"><span data-stu-id="208a3-115">PendingMailTips</span></span>](pendingmailtips.md) <br/> |<span data-ttu-id="208a3-116">Indica que as dicas de email neste elemento não puderam ser avaliadas antes que o tempo limite de processamento do servidor tenha expirado.</span><span class="sxs-lookup"><span data-stu-id="208a3-116">Indicates that the mail tips in this element could not be evaluated before the server's processing timeout expired.</span></span>  <br/> |
|[<span data-ttu-id="208a3-117">Fora</span><span class="sxs-lookup"><span data-stu-id="208a3-117">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="208a3-118">Representa a mensagem de resposta e um tempo de duração para envio da mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="208a3-118">Represents the response message and a duration time for sending the response message.</span></span>  <br/> |
|[<span data-ttu-id="208a3-119">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="208a3-119">MailboxFull</span></span>](mailboxfull.md) <br/> |<span data-ttu-id="208a3-120">Indica se a caixa de correio do destinatário está cheia.</span><span class="sxs-lookup"><span data-stu-id="208a3-120">Indicates whether the mailbox for the recipient is full.</span></span>  <br/> |
|[<span data-ttu-id="208a3-121">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="208a3-121">CustomMailTip</span></span>](custommailtip.md) <br/> |<span data-ttu-id="208a3-122">Representa uma mensagem de dica de email personalizada.</span><span class="sxs-lookup"><span data-stu-id="208a3-122">Represents a customized mail tip message.</span></span>  <br/> |
|[<span data-ttu-id="208a3-123">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="208a3-123">TotalMemberCount</span></span>](totalmembercount.md) <br/> |<span data-ttu-id="208a3-124">Representa a contagem de todos os membros de um grupo.</span><span class="sxs-lookup"><span data-stu-id="208a3-124">Represents the count of all members in a group.</span></span>  <br/> |
|[<span data-ttu-id="208a3-125">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="208a3-125">ExternalMemberCount</span></span>](externalmembercount.md) <br/> |<span data-ttu-id="208a3-126">Representa a contagem de membros externos em um grupo.</span><span class="sxs-lookup"><span data-stu-id="208a3-126">Represents the count of external members in a group.</span></span>  <br/> |
|[<span data-ttu-id="208a3-127">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="208a3-127">MaxMessageSize</span></span>](maxmessagesize.md) <br/> |<span data-ttu-id="208a3-128">Representa o tamanho máximo de mensagem que o destinatário pode aceitar.</span><span class="sxs-lookup"><span data-stu-id="208a3-128">Represents the maximum message size the recipient can accept.</span></span>  <br/> |
|[<span data-ttu-id="208a3-129">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="208a3-129">DeliveryRestricted</span></span>](deliveryrestricted.md) <br/> |<span data-ttu-id="208a3-130">Indica se as restrições de entrega impedirão que a mensagem do remetente atinja o destinatário.</span><span class="sxs-lookup"><span data-stu-id="208a3-130">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|[<span data-ttu-id="208a3-131">Ismoderadod</span><span class="sxs-lookup"><span data-stu-id="208a3-131">IsModerated</span></span>](ismoderated.md) <br/> |<span data-ttu-id="208a3-132">Indica se a caixa de correio do destinatário está sendo moderada.</span><span class="sxs-lookup"><span data-stu-id="208a3-132">Indicates whether the recipient's mailbox is being moderated.</span></span>  <br/> |
|[<span data-ttu-id="208a3-133">InvalidRecipient (dicas de dicas)</span><span class="sxs-lookup"><span data-stu-id="208a3-133">InvalidRecipient (MailTips)</span></span>](invalidrecipient-mailtips.md) <br/> |<span data-ttu-id="208a3-134">Indica se o destinatário é inválido.</span><span class="sxs-lookup"><span data-stu-id="208a3-134">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="208a3-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="208a3-135">Parent elements</span></span>

|<span data-ttu-id="208a3-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="208a3-136">**Element**</span></span>|<span data-ttu-id="208a3-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="208a3-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="208a3-138">MailTipsResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="208a3-138">MailTipsResponseMessageType</span></span>](mailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="208a3-139">Representa configurações de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="208a3-139">Represents mail tips settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="208a3-140">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="208a3-140">Text value</span></span>

<span data-ttu-id="208a3-141">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="208a3-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="208a3-142">Comentários</span><span class="sxs-lookup"><span data-stu-id="208a3-142">Remarks</span></span>

<span data-ttu-id="208a3-143">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="208a3-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="208a3-144">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="208a3-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="208a3-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="208a3-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="208a3-146">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="208a3-146">Schema Name</span></span>  <br/> |<span data-ttu-id="208a3-147">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="208a3-147">Messages schema</span></span>  <br/> |
|<span data-ttu-id="208a3-148">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="208a3-148">Validation File</span></span>  <br/> |<span data-ttu-id="208a3-149">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="208a3-149">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="208a3-150">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="208a3-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="208a3-151">False</span><span class="sxs-lookup"><span data-stu-id="208a3-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="208a3-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="208a3-152">See also</span></span>



- [<span data-ttu-id="208a3-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="208a3-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

