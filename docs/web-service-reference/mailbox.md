---
title: Mailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Mailbox
api_type:
- schema
ms.assetid: befc70fd-51cb-4258-884c-80c9050f0e82
description: O elemento de caixa de correio identifica um objeto do Active Directory habilitado para email.
ms.openlocfilehash: e9fa21f3678249a9ac13d567b88beaf0177f989f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824258"
---
# <a name="mailbox"></a><span data-ttu-id="46310-103">Mailbox</span><span class="sxs-lookup"><span data-stu-id="46310-103">Mailbox</span></span>

<span data-ttu-id="46310-104">O elemento de **caixa de correio** identifica um objeto do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="46310-104">The **Mailbox** element identifies a mail-enabled Active Directory object.</span></span> 
  
```XML
<Mailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Mailbox>
```

<span data-ttu-id="46310-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="46310-105">**EmailAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="46310-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="46310-106">Attributes and elements</span></span>

<span data-ttu-id="46310-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="46310-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46310-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="46310-108">Attributes</span></span>

<span data-ttu-id="46310-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="46310-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="46310-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="46310-110">Child elements</span></span>

|<span data-ttu-id="46310-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="46310-111">**Element**</span></span>|<span data-ttu-id="46310-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="46310-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46310-113">Nome (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="46310-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="46310-114">Define o nome do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="46310-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="46310-115">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="46310-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="46310-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="46310-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="46310-117">Define o endereço de Simple Mail Transfer Protocol (SMTP) de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="46310-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="46310-118">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="46310-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="46310-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="46310-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="46310-120">Define o roteamento que é usado para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="46310-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="46310-121">O padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="46310-121">The default is SMTP.</span></span> <span data-ttu-id="46310-122">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="46310-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="46310-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="46310-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="46310-124">Define o tipo de caixa de correio de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="46310-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="46310-125">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="46310-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="46310-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="46310-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="46310-127">Define o identificador do item de um contato ou uma lista de distribuição particular para destinatários da pasta de contatos do usuário.</span><span class="sxs-lookup"><span data-stu-id="46310-127">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="46310-128">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="46310-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="46310-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="46310-129">Parent elements</span></span>

|<span data-ttu-id="46310-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="46310-130">**Element**</span></span>|<span data-ttu-id="46310-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="46310-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46310-132">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="46310-132">ExpandDL</span></span>](expanddl.md) <br/> |<span data-ttu-id="46310-133">Define uma solicitação para expandir uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="46310-133">Defines a request to expand a distribution list.</span></span> <br/> <br/> <span data-ttu-id="46310-134">Este é a expressão XPath para esse elemento:` /ExpandDL `</span><span class="sxs-lookup"><span data-stu-id="46310-134">The following is the XPath expression to this element: ` /ExpandDL `</span></span> <br/> |
|[<span data-ttu-id="46310-135">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="46310-135">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="46310-136">Contém uma matriz de destinatários de um item.</span><span class="sxs-lookup"><span data-stu-id="46310-136">Contains an array of recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="46310-137">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="46310-137">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="46310-138">Representa uma coleção dos destinatários que receberão uma cópia da mensagem.</span><span class="sxs-lookup"><span data-stu-id="46310-138">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="46310-139">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="46310-139">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="46310-140">Representa uma coleção de destinatários para receber uma cópia oculta (Cco) de um email.</span><span class="sxs-lookup"><span data-stu-id="46310-140">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="46310-141">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="46310-141">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="46310-142">Identifica uma matriz de endereços de email para o qual as respostas devem ser enviadas.</span><span class="sxs-lookup"><span data-stu-id="46310-142">Identifies an array of e-mail addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="46310-143">Sender</span><span class="sxs-lookup"><span data-stu-id="46310-143">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="46310-144">Identifica o remetente de um item.</span><span class="sxs-lookup"><span data-stu-id="46310-144">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="46310-145">From</span><span class="sxs-lookup"><span data-stu-id="46310-145">From</span></span>](from.md) <br/> |<span data-ttu-id="46310-146">Representa o destinatário de quem a mensagem foi enviada.</span><span class="sxs-lookup"><span data-stu-id="46310-146">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="46310-147">Organizer</span><span class="sxs-lookup"><span data-stu-id="46310-147">Organizer</span></span>](organizer.md) <br/> |<span data-ttu-id="46310-148">Representa o organizador de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="46310-148">Represents the organizer of a meeting.</span></span>  <br/> |
|[<span data-ttu-id="46310-149">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="46310-149">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> | <span data-ttu-id="46310-150">Identifica as pastas padrão do Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="46310-150">Identifies default Microsoft Exchange Server 2007 folders.</span></span>  <br/><br/>  <span data-ttu-id="46310-151">A seguir estão as expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="46310-151">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/CreateItem/ParentFolderId/DistinguishedFolderId` <br/>  `/CreateFolder/ParentFolderId/DistinguishedFolderId` <br/> |
|[<span data-ttu-id="46310-152">Resolução</span><span class="sxs-lookup"><span data-stu-id="46310-152">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="46310-153">Contém uma única entidade resolvida.</span><span class="sxs-lookup"><span data-stu-id="46310-153">Contains a single resolved entity.</span></span>  <br/> |
|[<span data-ttu-id="46310-154">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="46310-154">DLExpansion</span></span>](dlexpansion.md) <br/> |<span data-ttu-id="46310-155">Contém uma matriz de caixas de correio que estão contidos em uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="46310-155">Contains an array of mailboxes that are contained in a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="46310-156">Attendee</span><span class="sxs-lookup"><span data-stu-id="46310-156">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="46310-157">Representa os participantes e recursos para um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="46310-157">Represents attendees and resources for a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="46310-158">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="46310-158">CreateManagedFolder</span></span>](createmanagedfolder.md) <br/> |<span data-ttu-id="46310-159">Define uma solicitação para adicionar pastas gerenciadas para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="46310-159">Defines a request to add managed folders to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="46310-160">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="46310-160">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="46310-161">Define uma solicitação para adicionar representantes para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="46310-161">Defines a request to add delegates to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="46310-162">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="46310-162">GetDelegate</span></span>](getdelegate.md) <br/> |<span data-ttu-id="46310-163">Define uma solicitação para obter mais informações sobre os representantes para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="46310-163">Defines a request to get information about delegates to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="46310-164">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="46310-164">RemoveDelegate</span></span>](removedelegate.md) <br/> |<span data-ttu-id="46310-165">Define uma solicitação para remover representantes de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="46310-165">Defines a request to remove delegates from a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="46310-166">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="46310-166">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="46310-167">Define uma solicitação de atualização de representantes em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="46310-167">Defines a request to update delegates in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="46310-168">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="46310-168">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="46310-169">Descreve o delegado em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="46310-169">Describes the delegate in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="46310-170">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="46310-170">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="46310-171">Descreve a entidade em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="46310-171">Describes the principal in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="46310-172">Membro</span><span class="sxs-lookup"><span data-stu-id="46310-172">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="46310-173">Representa um membro de uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="46310-173">Represents a member of a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="46310-174">Text value</span><span class="sxs-lookup"><span data-stu-id="46310-174">Text value</span></span>

<span data-ttu-id="46310-175">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="46310-175">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="46310-176">Comentários</span><span class="sxs-lookup"><span data-stu-id="46310-176">Remarks</span></span>

<span data-ttu-id="46310-177">Os elementos [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) e [ItemId](itemid.md) identificam uma lista de distribuição ou de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="46310-177">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) and [ItemId](itemid.md) elements identify a mailbox or distribution list.</span></span> 

<span data-ttu-id="46310-178">O elemento [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) identifica uma lista de distribuição ou de caixa de correio pelo endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="46310-178">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element identifies a mailbox or distribution list by SMTP address.</span></span> 

<span data-ttu-id="46310-179">O elemento [ItemId](itemid.md) identifica uma caixa de correio por um identificador de item, que é associado a uma caixa de correio específica.</span><span class="sxs-lookup"><span data-stu-id="46310-179">The [ItemId](itemid.md) element identifies a mailbox by an item identifier, which is associated with a particular mailbox.</span></span> 

<span data-ttu-id="46310-180">O elemento [ItemId](itemid.md) não pode ser usado para enviar uma mensagem para uma lista de distribuição ou um contato em uma pasta pública de contatos.</span><span class="sxs-lookup"><span data-stu-id="46310-180">The [ItemId](itemid.md) element cannot be used for sending a message to a distribution list or a contact in a public contacts folder.</span></span> <span data-ttu-id="46310-181">Um erro será lançado se isso for usado em uma operação de CreateItem, UpdateItem ou SendItem quando é feita uma tentativa para enviar uma mensagem a uma lista de distribuição ou um contato em uma pasta pública de contatos.</span><span class="sxs-lookup"><span data-stu-id="46310-181">An error will be thrown if this is used in a CreateItem, UpdateItem, or SendItem operation when an attempt is made to send a message to a distribution list or contact in a contacts public folder.</span></span> <span data-ttu-id="46310-182">Use a operação ExpandDL para obter o endereço SMTP e, em seguida, envie a mensagem usando o elemento [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) em vez do elemento [ItemId](itemid.md) .</span><span class="sxs-lookup"><span data-stu-id="46310-182">Use the ExpandDL operation to get the SMTP address and then send the message by using the [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element instead of the [ItemId](itemid.md) element.</span></span> 
  
<span data-ttu-id="46310-183">Outro elemento, [a caixa de correio (disponibilidade)](mailbox-availability.md), fornece informações para operações de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="46310-183">Another element, [Mailbox (Availability)](mailbox-availability.md), provides information for availability operations.</span></span> 
  
<span data-ttu-id="46310-184">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="46310-184">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46310-185">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="46310-185">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46310-186">Namespace</span><span class="sxs-lookup"><span data-stu-id="46310-186">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="46310-187">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="46310-187">Schema Name</span></span>  <br/> |<span data-ttu-id="46310-188">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="46310-188">Types schema</span></span>  <br/> |
|<span data-ttu-id="46310-189">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="46310-189">Validation File</span></span>  <br/> |<span data-ttu-id="46310-190">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="46310-190">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="46310-191">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="46310-191">Can be Empty</span></span>  <br/> |<span data-ttu-id="46310-192">False</span><span class="sxs-lookup"><span data-stu-id="46310-192">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="46310-193">Ver também</span><span class="sxs-lookup"><span data-stu-id="46310-193">See also</span></span>

- [<span data-ttu-id="46310-194">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="46310-194">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

