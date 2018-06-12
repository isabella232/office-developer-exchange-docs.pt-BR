---
title: Remetente (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Sender
api_type:
- schema
ms.assetid: 717eb6d0-d167-4b20-92e2-5d08b96186c4
description: O elemento de remetente representa o endereço de email para o remetente da mensagem.
ms.openlocfilehash: bac62412caf1044c13015f1d9d7ef63552747c1c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825320"
---
# <a name="sender-emailaddresstype"></a><span data-ttu-id="2b9ca-103">Remetente (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="2b9ca-103">Sender (EmailAddressType)</span></span>

<span data-ttu-id="2b9ca-104">O elemento de **remetente** representa o endereço de email para o remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="2b9ca-104">The **Sender** element represents the e-mail address for the sender of the message.</span></span> 
  
```XML
<Sender>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Sender>
```

 <span data-ttu-id="2b9ca-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="2b9ca-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b9ca-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2b9ca-106">Attributes and elements</span></span>

<span data-ttu-id="2b9ca-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2b9ca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b9ca-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2b9ca-108">Attributes</span></span>

<span data-ttu-id="2b9ca-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2b9ca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2b9ca-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2b9ca-110">Child elements</span></span>

|<span data-ttu-id="2b9ca-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2b9ca-111">**Element**</span></span>|<span data-ttu-id="2b9ca-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2b9ca-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b9ca-113">Nome (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="2b9ca-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="2b9ca-114">Representa o nome do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2b9ca-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="2b9ca-115">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="2b9ca-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="2b9ca-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="2b9ca-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="2b9ca-117">Define o endereço de Simple Mail Transfer Protocol (SMTP) principal de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2b9ca-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="2b9ca-118">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="2b9ca-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="2b9ca-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="2b9ca-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="2b9ca-120">Representa o protocolo de roteamento para o destinatário.</span><span class="sxs-lookup"><span data-stu-id="2b9ca-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="2b9ca-121">O valor padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="2b9ca-121">The default value is SMTP.</span></span> <span data-ttu-id="2b9ca-122">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="2b9ca-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="2b9ca-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="2b9ca-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="2b9ca-124">Representa o tipo de caixa de correio que é representado por um endereço de email.</span><span class="sxs-lookup"><span data-stu-id="2b9ca-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="2b9ca-125">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="2b9ca-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="2b9ca-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="2b9ca-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="2b9ca-127">Define o identificador do item de um contato ou uma lista de distribuição particular para destinatários da pasta de contatos do usuário.</span><span class="sxs-lookup"><span data-stu-id="2b9ca-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="2b9ca-128">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="2b9ca-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2b9ca-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2b9ca-129">Parent elements</span></span>

|<span data-ttu-id="2b9ca-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2b9ca-130">**Element**</span></span>|<span data-ttu-id="2b9ca-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2b9ca-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b9ca-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="2b9ca-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="2b9ca-133">Especifica os critérios para os tipos de mensagens para encontrar.</span><span class="sxs-lookup"><span data-stu-id="2b9ca-133">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="2b9ca-134">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="2b9ca-134">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="2b9ca-135">Contém um resultado de mensagem única de um elemento [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="2b9ca-135">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
|[<span data-ttu-id="2b9ca-136">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="2b9ca-136">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="2b9ca-137">Contém uma única mensagem retornada em uma [operação de GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="2b9ca-137">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2b9ca-138">Text value</span><span class="sxs-lookup"><span data-stu-id="2b9ca-138">Text value</span></span>

<span data-ttu-id="2b9ca-139">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2b9ca-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2b9ca-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="2b9ca-140">Remarks</span></span>

<span data-ttu-id="2b9ca-141">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2b9ca-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b9ca-142">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2b9ca-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b9ca-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="2b9ca-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2b9ca-144">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2b9ca-144">Schema Name</span></span>  <br/> |<span data-ttu-id="2b9ca-145">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="2b9ca-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="2b9ca-146">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2b9ca-146">Validation File</span></span>  <br/> |<span data-ttu-id="2b9ca-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2b9ca-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2b9ca-148">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2b9ca-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="2b9ca-149">False</span><span class="sxs-lookup"><span data-stu-id="2b9ca-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2b9ca-150">Ver também</span><span class="sxs-lookup"><span data-stu-id="2b9ca-150">See also</span></span>



[<span data-ttu-id="2b9ca-151">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="2b9ca-151">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="2b9ca-152">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2b9ca-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

