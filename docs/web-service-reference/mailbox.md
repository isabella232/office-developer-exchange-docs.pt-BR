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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824258"
---
# <a name="mailbox"></a><span data-ttu-id="b86d7-103">Mailbox</span><span class="sxs-lookup"><span data-stu-id="b86d7-103">Mailbox</span></span>

<span data-ttu-id="b86d7-104">O elemento de **caixa de correio** identifica um objeto do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="b86d7-104">The **Mailbox** element identifies a mail-enabled Active Directory object.</span></span> 
  
```XML
<Mailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Mailbox>
```

<span data-ttu-id="b86d7-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="b86d7-105">**EmailAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b86d7-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b86d7-106">Attributes and elements</span></span>

<span data-ttu-id="b86d7-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b86d7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b86d7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b86d7-108">Attributes</span></span>

<span data-ttu-id="b86d7-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b86d7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b86d7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b86d7-110">Child elements</span></span>

|<span data-ttu-id="b86d7-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b86d7-111">**Element**</span></span>|<span data-ttu-id="b86d7-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b86d7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b86d7-113">Nome (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="b86d7-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="b86d7-114">Define o nome do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b86d7-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="b86d7-115">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="b86d7-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="b86d7-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="b86d7-117">Define o endereço de Simple Mail Transfer Protocol (SMTP) de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b86d7-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="b86d7-118">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="b86d7-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="b86d7-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="b86d7-120">Define o roteamento que é usado para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b86d7-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="b86d7-121">O padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="b86d7-121">The default is SMTP.</span></span> <span data-ttu-id="b86d7-122">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="b86d7-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="b86d7-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="b86d7-124">Define o tipo de caixa de correio de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b86d7-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="b86d7-125">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="b86d7-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="b86d7-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="b86d7-127">Define o identificador do item de um contato ou uma lista de distribuição particular para destinatários da pasta de contatos do usuário.</span><span class="sxs-lookup"><span data-stu-id="b86d7-127">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="b86d7-128">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="b86d7-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b86d7-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b86d7-129">Parent elements</span></span>

|<span data-ttu-id="b86d7-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b86d7-130">**Element**</span></span>|<span data-ttu-id="b86d7-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b86d7-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b86d7-132">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="b86d7-132">ExpandDL</span></span>](expanddl.md) <br/> |<span data-ttu-id="b86d7-133">Define uma solicitação para expandir uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="b86d7-133">Defines a request to expand a distribution list.</span></span> <br/> <br/> <span data-ttu-id="b86d7-134">Este é a expressão XPath para esse elemento:` /ExpandDL `</span><span class="sxs-lookup"><span data-stu-id="b86d7-134">The following is the XPath expression to this element: ` /ExpandDL `</span></span> <br/> |
|[<span data-ttu-id="b86d7-135">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="b86d7-135">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="b86d7-136">Contém uma matriz de destinatários de um item.</span><span class="sxs-lookup"><span data-stu-id="b86d7-136">Contains an array of recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-137">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="b86d7-137">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="b86d7-138">Representa uma coleção dos destinatários que receberão uma cópia da mensagem.</span><span class="sxs-lookup"><span data-stu-id="b86d7-138">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-139">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="b86d7-139">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="b86d7-140">Representa uma coleção de destinatários para receber uma cópia oculta (Cco) de um email.</span><span class="sxs-lookup"><span data-stu-id="b86d7-140">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-141">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="b86d7-141">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="b86d7-142">Identifica uma matriz de endereços de email para o qual as respostas devem ser enviadas.</span><span class="sxs-lookup"><span data-stu-id="b86d7-142">Identifies an array of e-mail addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-143">Sender</span><span class="sxs-lookup"><span data-stu-id="b86d7-143">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="b86d7-144">Identifica o remetente de um item.</span><span class="sxs-lookup"><span data-stu-id="b86d7-144">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-145">From</span><span class="sxs-lookup"><span data-stu-id="b86d7-145">From</span></span>](from.md) <br/> |<span data-ttu-id="b86d7-146">Representa o destinatário de quem a mensagem foi enviada.</span><span class="sxs-lookup"><span data-stu-id="b86d7-146">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-147">Organizer</span><span class="sxs-lookup"><span data-stu-id="b86d7-147">Organizer</span></span>](organizer.md) <br/> |<span data-ttu-id="b86d7-148">Representa o organizador de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="b86d7-148">Represents the organizer of a meeting.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-149">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="b86d7-149">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> | <span data-ttu-id="b86d7-150">Identifica as pastas padrão do Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="b86d7-150">Identifies default Microsoft Exchange Server 2007 folders.</span></span>  <br/><br/>  <span data-ttu-id="b86d7-151">A seguir estão as expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="b86d7-151">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/CreateItem/ParentFolderId/DistinguishedFolderId` <br/>  `/CreateFolder/ParentFolderId/DistinguishedFolderId` <br/> |
|[<span data-ttu-id="b86d7-152">Resolução</span><span class="sxs-lookup"><span data-stu-id="b86d7-152">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="b86d7-153">Contém uma única entidade resolvida.</span><span class="sxs-lookup"><span data-stu-id="b86d7-153">Contains a single resolved entity.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-154">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="b86d7-154">DLExpansion</span></span>](dlexpansion.md) <br/> |<span data-ttu-id="b86d7-155">Contém uma matriz de caixas de correio que estão contidos em uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="b86d7-155">Contains an array of mailboxes that are contained in a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-156">Attendee</span><span class="sxs-lookup"><span data-stu-id="b86d7-156">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="b86d7-157">Representa os participantes e recursos para um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="b86d7-157">Represents attendees and resources for a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-158">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="b86d7-158">CreateManagedFolder</span></span>](createmanagedfolder.md) <br/> |<span data-ttu-id="b86d7-159">Define uma solicitação para adicionar pastas gerenciadas para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b86d7-159">Defines a request to add managed folders to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-160">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="b86d7-160">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="b86d7-161">Define uma solicitação para adicionar representantes para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b86d7-161">Defines a request to add delegates to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-162">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="b86d7-162">GetDelegate</span></span>](getdelegate.md) <br/> |<span data-ttu-id="b86d7-163">Define uma solicitação para obter mais informações sobre os representantes para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b86d7-163">Defines a request to get information about delegates to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-164">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="b86d7-164">RemoveDelegate</span></span>](removedelegate.md) <br/> |<span data-ttu-id="b86d7-165">Define uma solicitação para remover representantes de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b86d7-165">Defines a request to remove delegates from a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-166">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="b86d7-166">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="b86d7-167">Define uma solicitação de atualização de representantes em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b86d7-167">Defines a request to update delegates in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-168">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="b86d7-168">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="b86d7-169">Descreve o delegado em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="b86d7-169">Describes the delegate in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-170">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="b86d7-170">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="b86d7-171">Descreve a entidade em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="b86d7-171">Describes the principal in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="b86d7-172">Membro</span><span class="sxs-lookup"><span data-stu-id="b86d7-172">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b86d7-173">Representa um membro de uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="b86d7-173">Represents a member of a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b86d7-174">Text value</span><span class="sxs-lookup"><span data-stu-id="b86d7-174">Text value</span></span>

<span data-ttu-id="b86d7-175">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b86d7-175">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b86d7-176">Comentários</span><span class="sxs-lookup"><span data-stu-id="b86d7-176">Remarks</span></span>

<span data-ttu-id="b86d7-177">Os elementos [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) e [ItemId](itemid.md) identificam uma lista de distribuição ou de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b86d7-177">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) and [ItemId](itemid.md) elements identify a mailbox or distribution list.</span></span> 

<span data-ttu-id="b86d7-178">O elemento [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) identifica uma lista de distribuição ou de caixa de correio pelo endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="b86d7-178">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element identifies a mailbox or distribution list by SMTP address.</span></span> 

<span data-ttu-id="b86d7-179">O elemento [ItemId](itemid.md) identifica uma caixa de correio por um identificador de item, que é associado a uma caixa de correio específica.</span><span class="sxs-lookup"><span data-stu-id="b86d7-179">The [ItemId](itemid.md) element identifies a mailbox by an item identifier, which is associated with a particular mailbox.</span></span> 

<span data-ttu-id="b86d7-180">O elemento [ItemId](itemid.md) não pode ser usado para enviar uma mensagem para uma lista de distribuição ou um contato em uma pasta pública de contatos.</span><span class="sxs-lookup"><span data-stu-id="b86d7-180">The [ItemId](itemid.md) element cannot be used for sending a message to a distribution list or a contact in a public contacts folder.</span></span> <span data-ttu-id="b86d7-181">Um erro será lançado se isso for usado em uma operação de CreateItem, UpdateItem ou SendItem quando é feita uma tentativa para enviar uma mensagem a uma lista de distribuição ou um contato em uma pasta pública de contatos.</span><span class="sxs-lookup"><span data-stu-id="b86d7-181">An error will be thrown if this is used in a CreateItem, UpdateItem, or SendItem operation when an attempt is made to send a message to a distribution list or contact in a contacts public folder.</span></span> <span data-ttu-id="b86d7-182">Use a operação ExpandDL para obter o endereço SMTP e, em seguida, envie a mensagem usando o elemento [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) em vez do elemento [ItemId](itemid.md) .</span><span class="sxs-lookup"><span data-stu-id="b86d7-182">Use the ExpandDL operation to get the SMTP address and then send the message by using the [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element instead of the [ItemId](itemid.md) element.</span></span> 
  
<span data-ttu-id="b86d7-183">Outro elemento, [a caixa de correio (disponibilidade)](mailbox-availability.md), fornece informações para operações de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="b86d7-183">Another element, [Mailbox (Availability)](mailbox-availability.md), provides information for availability operations.</span></span> 
  
<span data-ttu-id="b86d7-184">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b86d7-184">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b86d7-185">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b86d7-185">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b86d7-186">Namespace</span><span class="sxs-lookup"><span data-stu-id="b86d7-186">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b86d7-187">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b86d7-187">Schema Name</span></span>  <br/> |<span data-ttu-id="b86d7-188">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b86d7-188">Types schema</span></span>  <br/> |
|<span data-ttu-id="b86d7-189">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b86d7-189">Validation File</span></span>  <br/> |<span data-ttu-id="b86d7-190">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b86d7-190">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b86d7-191">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b86d7-191">Can be Empty</span></span>  <br/> |<span data-ttu-id="b86d7-192">False</span><span class="sxs-lookup"><span data-stu-id="b86d7-192">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b86d7-193">Ver também</span><span class="sxs-lookup"><span data-stu-id="b86d7-193">See also</span></span>

- [<span data-ttu-id="b86d7-194">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b86d7-194">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

