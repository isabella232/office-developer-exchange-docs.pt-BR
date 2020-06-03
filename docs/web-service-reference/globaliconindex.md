---
title: GlobalIconIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d28ed70-4cfe-46e4-8d15-593c6e355bcf
description: O elemento GlobalIconIndex identifica o índice de ícone global de todos os itens em uma conversa.
ms.openlocfilehash: 9900a80136a1a7eaae4634afd31568679f6dba1b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459458"
---
# <a name="globaliconindex"></a><span data-ttu-id="5db53-103">GlobalIconIndex</span><span class="sxs-lookup"><span data-stu-id="5db53-103">GlobalIconIndex</span></span>

<span data-ttu-id="5db53-104">O elemento **GlobalIconIndex** identifica o índice de ícone global de todos os itens em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="5db53-104">The **GlobalIconIndex** element identifies the global icon index for all items in a conversation.</span></span> 
  
```XML
<IconIndex>Default | PostItem | MailRead | MailUnread | MailReplied | MailForwarded | MailEncrypted | MailSmimeSigned | MailEncrytedReplied | MailSmimeSignedReplied | MailEncryptedForwarded | MailSmimeSignedForwarded | MailEncryptedRead | MailSmimeSignedRead | MailIrm | MaillrmForwarded | MaillrmReplied | SmsSubmitted | SmsRoutedToDeliveryPoint | SmsRoutedToExternalMessagingSystem | SmsDelivered | OutlookDefaultForContacts | AppointmentItem | AppointmentRecur | AppointmentMeet | AppointmentMeetRecur | AppointmentMeetNY | AppointmentMeetYes | AppointmentMeetNo | AppointmentMeetMaybe | AppointmentMeetCancel | AppointmentMeetInfo | TaskItem | TaskRecur | TaskOwned | TaskDelegated</IconIndex>
```

 <span data-ttu-id="5db53-105">**IconIndexType**</span><span class="sxs-lookup"><span data-stu-id="5db53-105">**IconIndexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5db53-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5db53-106">Attributes and elements</span></span>

<span data-ttu-id="5db53-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5db53-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5db53-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5db53-108">Attributes</span></span>

<span data-ttu-id="5db53-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5db53-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5db53-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5db53-110">Child elements</span></span>

<span data-ttu-id="5db53-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5db53-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5db53-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5db53-112">Parent elements</span></span>

<span data-ttu-id="5db53-113">[Conversa (conversatype)](conversation-conversationtype.md)  |  [Item](item.md)  |  [Contato](contact.md)  |  [DistributionList](distributionlist.md)  |  [Mensagem](message-ex15websvcsotherref.md)  |  [CalendarItem](calendaritem.md)  |  [PostItem](postitem.md)  |  [Tarefa](task.md)</span><span class="sxs-lookup"><span data-stu-id="5db53-113">[Conversation (ConversationType)](conversation-conversationtype.md) | [Item](item.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Message](message-ex15websvcsotherref.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="5db53-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5db53-114">Text value</span></span>

<span data-ttu-id="5db53-115">A tabela a seguir contém os valores de texto possíveis para o elemento **GlobalIconIndex** .</span><span class="sxs-lookup"><span data-stu-id="5db53-115">The following table contains the possible text values for the **GlobalIconIndex** element.</span></span> 
  
|<span data-ttu-id="5db53-116">**Valor**</span><span class="sxs-lookup"><span data-stu-id="5db53-116">**Value**</span></span>|<span data-ttu-id="5db53-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5db53-117">**Description**</span></span>|
|:-----|:-----|
|||
|<span data-ttu-id="5db53-118">Padrão</span><span class="sxs-lookup"><span data-stu-id="5db53-118">Default</span></span>  <br/> |<span data-ttu-id="5db53-119">Especifica o ícone padrão.</span><span class="sxs-lookup"><span data-stu-id="5db53-119">Specifies the default icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-120">Item de postagem</span><span class="sxs-lookup"><span data-stu-id="5db53-120">PostItem</span></span>  <br/> |<span data-ttu-id="5db53-121">Especifica o ícone de um item de postagem.</span><span class="sxs-lookup"><span data-stu-id="5db53-121">Specifies the icon for a post item.</span></span>  <br/> |
|<span data-ttu-id="5db53-122">MailRead</span><span class="sxs-lookup"><span data-stu-id="5db53-122">MailRead</span></span>  <br/> |<span data-ttu-id="5db53-123">Especifica o ícone de leitura de email.</span><span class="sxs-lookup"><span data-stu-id="5db53-123">Specifies the mail read icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-124">MailUnread</span><span class="sxs-lookup"><span data-stu-id="5db53-124">MailUnread</span></span>  <br/> |<span data-ttu-id="5db53-125">Especifica o ícone de email não lido.</span><span class="sxs-lookup"><span data-stu-id="5db53-125">Specifies the unread mail icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-126">MailReplied</span><span class="sxs-lookup"><span data-stu-id="5db53-126">MailReplied</span></span>  <br/> |<span data-ttu-id="5db53-127">Especifica o ícone de email respondido.</span><span class="sxs-lookup"><span data-stu-id="5db53-127">Specifies the replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-128">MailForwarded</span><span class="sxs-lookup"><span data-stu-id="5db53-128">MailForwarded</span></span>  <br/> |<span data-ttu-id="5db53-129">Especifica o ícone de email encaminhado.</span><span class="sxs-lookup"><span data-stu-id="5db53-129">Specifies the forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-130">MailEncrypted</span><span class="sxs-lookup"><span data-stu-id="5db53-130">MailEncrypted</span></span>  <br/> |<span data-ttu-id="5db53-131">Especifica o ícone de email criptografado.</span><span class="sxs-lookup"><span data-stu-id="5db53-131">Specifies the encrypted mail icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-132">MailSmimeSigned</span><span class="sxs-lookup"><span data-stu-id="5db53-132">MailSmimeSigned</span></span>  <br/> |<span data-ttu-id="5db53-133">Especifica o ícone de email assinado S/MIME (Secure/Multipurpose Internet Mail Extensions).</span><span class="sxs-lookup"><span data-stu-id="5db53-133">Specifies the Secure/Multipurpose Internet Mail Extensions (S/MIME) signed mail icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-134">MailEncryptedReplied</span><span class="sxs-lookup"><span data-stu-id="5db53-134">MailEncryptedReplied</span></span>  <br/> |<span data-ttu-id="5db53-135">Especifica o ícone de resposta de email criptografado.</span><span class="sxs-lookup"><span data-stu-id="5db53-135">Specifies the encrypted replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-136">MailSmimeSignedReplied</span><span class="sxs-lookup"><span data-stu-id="5db53-136">MailSmimeSignedReplied</span></span>  <br/> |<span data-ttu-id="5db53-137">Especifica o ícone de email assinado por S/MIME.</span><span class="sxs-lookup"><span data-stu-id="5db53-137">Specifies the S/MIME signed replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-138">MailEncryptedForwarded</span><span class="sxs-lookup"><span data-stu-id="5db53-138">MailEncryptedForwarded</span></span>  <br/> |<span data-ttu-id="5db53-139">Especifica o ícone de email encaminhado criptografado.</span><span class="sxs-lookup"><span data-stu-id="5db53-139">Specifies the encrypted forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-140">MailSmimeSignedForwarded</span><span class="sxs-lookup"><span data-stu-id="5db53-140">MailSmimeSignedForwarded</span></span>  <br/> |<span data-ttu-id="5db53-141">Especifica o ícone de email enviado por S/MIME.</span><span class="sxs-lookup"><span data-stu-id="5db53-141">Specifies the S/MIME signed forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-142">MailEncryptedRead</span><span class="sxs-lookup"><span data-stu-id="5db53-142">MailEncryptedRead</span></span>  <br/> |<span data-ttu-id="5db53-143">Especifica o ícone criptografar emails lidos.</span><span class="sxs-lookup"><span data-stu-id="5db53-143">Specifies the encrypted read mail icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-144">MailSmimeSignedRead</span><span class="sxs-lookup"><span data-stu-id="5db53-144">MailSmimeSignedRead</span></span>  <br/> |<span data-ttu-id="5db53-145">Especifica o ícone de leitura/gravação assinada por S/MIME.</span><span class="sxs-lookup"><span data-stu-id="5db53-145">Specifies the S/MIME signed read mail icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-146">MailIrm</span><span class="sxs-lookup"><span data-stu-id="5db53-146">MailIrm</span></span>  <br/> |<span data-ttu-id="5db53-147">Especifica o ícone de email protegido pelo gerenciamento de direitos de informação (IRM).</span><span class="sxs-lookup"><span data-stu-id="5db53-147">Specifies the Information Rights Management (IRM)-protected mail icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-148">MailIrmForwarded</span><span class="sxs-lookup"><span data-stu-id="5db53-148">MailIrmForwarded</span></span>  <br/> |<span data-ttu-id="5db53-149">Especifica o ícone de email encaminhado protegido por IRM.</span><span class="sxs-lookup"><span data-stu-id="5db53-149">Specifies the IRM-protected forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-150">MailIrmReplied</span><span class="sxs-lookup"><span data-stu-id="5db53-150">MailIrmReplied</span></span>  <br/> |<span data-ttu-id="5db53-151">Especifica o ícone do email protegido por IRM.</span><span class="sxs-lookup"><span data-stu-id="5db53-151">Specifies the IRM-protected replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-152">SmsSubmitted</span><span class="sxs-lookup"><span data-stu-id="5db53-152">SmsSubmitted</span></span>  <br/> |<span data-ttu-id="5db53-153">Especifica o ícone de email enviado para roteamento de serviço de mensagens curtas (SMS).</span><span class="sxs-lookup"><span data-stu-id="5db53-153">Specifies the icon for mail submitted for Short Message Service (SMS) routing.</span></span>  <br/> |
|<span data-ttu-id="5db53-154">SmsRoutedToDeliveryPoint</span><span class="sxs-lookup"><span data-stu-id="5db53-154">SmsRoutedToDeliveryPoint</span></span>  <br/> |<span data-ttu-id="5db53-155">Especifica o ícone do roteamento do SMS para um ponto de entrega externo.</span><span class="sxs-lookup"><span data-stu-id="5db53-155">Specifies the icon for SMS routing to an external delivery point.</span></span>  <br/> |
|<span data-ttu-id="5db53-156">SmsRoutedToExternalMessagingSystem</span><span class="sxs-lookup"><span data-stu-id="5db53-156">SmsRoutedToExternalMessagingSystem</span></span>  <br/> |<span data-ttu-id="5db53-157">Especifica o ícone do roteamento do SMS para um sistema de mensagens externos.</span><span class="sxs-lookup"><span data-stu-id="5db53-157">Specifies the icon for SMS routing to an external messaging system.</span></span>  <br/> |
|<span data-ttu-id="5db53-158">SmsDelivered</span><span class="sxs-lookup"><span data-stu-id="5db53-158">SmsDelivered</span></span>  <br/> |<span data-ttu-id="5db53-159">Especifica o ícone de email entregue pelo SMS.</span><span class="sxs-lookup"><span data-stu-id="5db53-159">Specifies the SMS delivered mail icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-160">OutlookDefaultForContacts</span><span class="sxs-lookup"><span data-stu-id="5db53-160">OutlookDefaultForContacts</span></span>  <br/> |<span data-ttu-id="5db53-161">Especifica o ícone padrão para contatos.</span><span class="sxs-lookup"><span data-stu-id="5db53-161">Specifies the default icon for contacts.</span></span>  <br/> |
|<span data-ttu-id="5db53-162">AppointmentItem</span><span class="sxs-lookup"><span data-stu-id="5db53-162">AppointmentItem</span></span>  <br/> |<span data-ttu-id="5db53-163">Especifica o ícone de item de compromisso.</span><span class="sxs-lookup"><span data-stu-id="5db53-163">Specifies the appointment item icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-164">AppointmentRecur</span><span class="sxs-lookup"><span data-stu-id="5db53-164">AppointmentRecur</span></span>  <br/> |<span data-ttu-id="5db53-165">Especifica o ícone de compromisso recorrente.</span><span class="sxs-lookup"><span data-stu-id="5db53-165">Specifies the recurring appointment icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-166">AppointmentMeet</span><span class="sxs-lookup"><span data-stu-id="5db53-166">AppointmentMeet</span></span>  <br/> |<span data-ttu-id="5db53-167">Especifica o ícone da reunião.</span><span class="sxs-lookup"><span data-stu-id="5db53-167">Specifies the meeting icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-168">AppointmentMeetRecur</span><span class="sxs-lookup"><span data-stu-id="5db53-168">AppointmentMeetRecur</span></span>  <br/> |<span data-ttu-id="5db53-169">Especifica o ícone de reunião recorrente.</span><span class="sxs-lookup"><span data-stu-id="5db53-169">Specifies the recurring meeting icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-170">AppointmentMeetNY</span><span class="sxs-lookup"><span data-stu-id="5db53-170">AppointmentMeetNY</span></span>  <br/> |<span data-ttu-id="5db53-171">Especifica o ícone de uma resposta provisória à reunião.</span><span class="sxs-lookup"><span data-stu-id="5db53-171">Specifies the icon for a tentative response to the meeting.</span></span>  <br/> |
|<span data-ttu-id="5db53-172">AppointmentMeetYes</span><span class="sxs-lookup"><span data-stu-id="5db53-172">AppointmentMeetYes</span></span>  <br/> |<span data-ttu-id="5db53-173">Especifica o ícone de aceitação da reunião.</span><span class="sxs-lookup"><span data-stu-id="5db53-173">Specifies the meeting acceptance icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-174">AppointmentMeetNo</span><span class="sxs-lookup"><span data-stu-id="5db53-174">AppointmentMeetNo</span></span>  <br/> |<span data-ttu-id="5db53-175">Especifica o ícone de reunião recusada.</span><span class="sxs-lookup"><span data-stu-id="5db53-175">Specifies the meeting declined icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-176">AppointmentMeetMaybe</span><span class="sxs-lookup"><span data-stu-id="5db53-176">AppointmentMeetMaybe</span></span>  <br/> |<span data-ttu-id="5db53-177">Especifica o ícone de uma resposta da reunião.</span><span class="sxs-lookup"><span data-stu-id="5db53-177">Specifies the icon for a maybe response to the meeting.</span></span>  <br/> |
|<span data-ttu-id="5db53-178">AppointmentMeetCancel</span><span class="sxs-lookup"><span data-stu-id="5db53-178">AppointmentMeetCancel</span></span>  <br/> |<span data-ttu-id="5db53-179">Especifica o ícone de cancelamento da reunião.</span><span class="sxs-lookup"><span data-stu-id="5db53-179">Specifies the meeting cancel icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-180">AppointmentMeetInfo</span><span class="sxs-lookup"><span data-stu-id="5db53-180">AppointmentMeetInfo</span></span>  <br/> |<span data-ttu-id="5db53-181">Especifica o ícone de informações da reunião.</span><span class="sxs-lookup"><span data-stu-id="5db53-181">Specifies the meeting information icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-182">Item de tarefa</span><span class="sxs-lookup"><span data-stu-id="5db53-182">TaskItem</span></span>  <br/> |<span data-ttu-id="5db53-183">Especifica o ícone do item de tarefa.</span><span class="sxs-lookup"><span data-stu-id="5db53-183">Specifies the task item icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-184">TaskRecur</span><span class="sxs-lookup"><span data-stu-id="5db53-184">TaskRecur</span></span>  <br/> |<span data-ttu-id="5db53-185">Especifica o ícone de tarefa recorrente.</span><span class="sxs-lookup"><span data-stu-id="5db53-185">Specifies the recurring task icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-186">TaskOwned</span><span class="sxs-lookup"><span data-stu-id="5db53-186">TaskOwned</span></span>  <br/> |<span data-ttu-id="5db53-187">Especifica o ícone de propriedade da tarefa.</span><span class="sxs-lookup"><span data-stu-id="5db53-187">Specifies the task owned icon.</span></span>  <br/> |
|<span data-ttu-id="5db53-188">TaskDelegated</span><span class="sxs-lookup"><span data-stu-id="5db53-188">TaskDelegated</span></span>  <br/> |<span data-ttu-id="5db53-189">Especifica o ícone delegado da tarefa.</span><span class="sxs-lookup"><span data-stu-id="5db53-189">Specifies the task delegated icon.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5db53-190">Comentários</span><span class="sxs-lookup"><span data-stu-id="5db53-190">Remarks</span></span>

<span data-ttu-id="5db53-191">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5db53-191">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5db53-192">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5db53-192">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5db53-193">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5db53-193">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5db53-194">Namespace</span><span class="sxs-lookup"><span data-stu-id="5db53-194">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5db53-195">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5db53-195">Schema name</span></span>  <br/> |<span data-ttu-id="5db53-196">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5db53-196">Types schema</span></span>  <br/> |
|<span data-ttu-id="5db53-197">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5db53-197">Validation file</span></span>  <br/> |<span data-ttu-id="5db53-198">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5db53-198">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5db53-199">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="5db53-199">Can be empty</span></span>  <br/> |<span data-ttu-id="5db53-200">falso</span><span class="sxs-lookup"><span data-stu-id="5db53-200">false</span></span>  <br/> |
   

