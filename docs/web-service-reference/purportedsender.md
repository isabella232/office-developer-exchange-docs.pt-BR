---
title: PurportedSender
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PurportedSender
api_type:
- schema
ms.assetid: eb7a54ec-2e48-4030-bbcf-50a31609691b
description: O elemento PurportedSender contém informações de contato para o suposto remetente de uma mensagem de email.
ms.openlocfilehash: 5ecf352484a423e3955736620bf5a65c4e98099a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468331"
---
# <a name="purportedsender"></a><span data-ttu-id="702c0-103">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="702c0-103">PurportedSender</span></span>

<span data-ttu-id="702c0-104">O elemento **PurportedSender** contém informações de contato para o suposto remetente de uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="702c0-104">The **PurportedSender** element contains contact information for the alleged sender of an e-mail message.</span></span> 
  
```XML
<PurportedSender>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</PurportedSender>
```

 <span data-ttu-id="702c0-105">**EmailAddresstype**</span><span class="sxs-lookup"><span data-stu-id="702c0-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="702c0-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="702c0-106">Attributes and elements</span></span>

<span data-ttu-id="702c0-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="702c0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="702c0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="702c0-108">Attributes</span></span>

<span data-ttu-id="702c0-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="702c0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="702c0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="702c0-110">Child elements</span></span>

|<span data-ttu-id="702c0-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="702c0-111">**Element**</span></span>|<span data-ttu-id="702c0-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="702c0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="702c0-113">Nome (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="702c0-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="702c0-114">Representa o nome do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="702c0-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="702c0-115">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="702c0-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="702c0-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="702c0-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="702c0-117">Define o endereço SMTP (Simple Mail Transfer Protocol) de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="702c0-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="702c0-118">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="702c0-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="702c0-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="702c0-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="702c0-120">Representa o protocolo de roteamento para o destinatário.</span><span class="sxs-lookup"><span data-stu-id="702c0-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="702c0-121">O valor padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="702c0-121">The default value is SMTP.</span></span> <span data-ttu-id="702c0-122">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="702c0-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="702c0-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="702c0-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="702c0-124">Representa o tipo de caixa de correio que é representado pelo endereço de email..</span><span class="sxs-lookup"><span data-stu-id="702c0-124">Represents the type of mailbox that is represented by the e-mail address..</span></span> <span data-ttu-id="702c0-125">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="702c0-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="702c0-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="702c0-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="702c0-127">Define o identificador de item de um contato ou de uma lista de distribuição privada para destinatários da pasta contatos de um usuário.</span><span class="sxs-lookup"><span data-stu-id="702c0-127">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="702c0-128">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="702c0-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="702c0-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="702c0-129">Parent elements</span></span>

|<span data-ttu-id="702c0-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="702c0-130">**Element**</span></span>|<span data-ttu-id="702c0-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="702c0-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="702c0-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="702c0-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="702c0-133">Especifica critérios para os tipos de mensagens a serem encontradas.</span><span class="sxs-lookup"><span data-stu-id="702c0-133">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="702c0-134">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="702c0-134">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="702c0-135">Contém uma única mensagem que é retornada em uma [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="702c0-135">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="702c0-136">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="702c0-136">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="702c0-137">Contém um único resultado de mensagem para um elemento [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="702c0-137">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="702c0-138">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="702c0-138">Text value</span></span>

<span data-ttu-id="702c0-139">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="702c0-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="702c0-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="702c0-140">Remarks</span></span>

<span data-ttu-id="702c0-141">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="702c0-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="702c0-142">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="702c0-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="702c0-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="702c0-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="702c0-144">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="702c0-144">Schema Name</span></span>  <br/> |<span data-ttu-id="702c0-145">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="702c0-145">Messages schema</span></span>  <br/> |
|<span data-ttu-id="702c0-146">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="702c0-146">Validation File</span></span>  <br/> |<span data-ttu-id="702c0-147">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="702c0-147">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="702c0-148">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="702c0-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="702c0-149">False</span><span class="sxs-lookup"><span data-stu-id="702c0-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="702c0-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="702c0-150">See also</span></span>



[<span data-ttu-id="702c0-151">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="702c0-151">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="702c0-152">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="702c0-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

