---
title: Remetente (EmailAddresstype)
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
description: O elemento Sender representa o endereço de email do remetente da mensagem.
ms.openlocfilehash: 23a487f216a110796d40f3d3e86224c691acc004
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455321"
---
# <a name="sender-emailaddresstype"></a><span data-ttu-id="f816a-103">Remetente (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="f816a-103">Sender (EmailAddressType)</span></span>

<span data-ttu-id="f816a-104">O elemento **Sender** representa o endereço de email do remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="f816a-104">The **Sender** element represents the e-mail address for the sender of the message.</span></span> 
  
```XML
<Sender>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Sender>
```

 <span data-ttu-id="f816a-105">**EmailAddresstype**</span><span class="sxs-lookup"><span data-stu-id="f816a-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f816a-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f816a-106">Attributes and elements</span></span>

<span data-ttu-id="f816a-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f816a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f816a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f816a-108">Attributes</span></span>

<span data-ttu-id="f816a-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f816a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f816a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f816a-110">Child elements</span></span>

|<span data-ttu-id="f816a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f816a-111">**Element**</span></span>|<span data-ttu-id="f816a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f816a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f816a-113">Nome (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="f816a-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="f816a-114">Representa o nome do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f816a-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="f816a-115">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="f816a-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="f816a-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="f816a-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="f816a-117">Define o endereço SMTP (Simple Mail Transfer Protocol) principal de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f816a-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="f816a-118">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="f816a-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="f816a-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="f816a-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="f816a-120">Representa o protocolo de roteamento para o destinatário.</span><span class="sxs-lookup"><span data-stu-id="f816a-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="f816a-121">O valor padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="f816a-121">The default value is SMTP.</span></span> <span data-ttu-id="f816a-122">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="f816a-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="f816a-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="f816a-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="f816a-124">Representa o tipo de caixa de correio que é representado pelo endereço de email.</span><span class="sxs-lookup"><span data-stu-id="f816a-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="f816a-125">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="f816a-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="f816a-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="f816a-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="f816a-127">Define o identificador de item de um contato ou de uma lista de distribuição privada para destinatários da pasta contatos de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f816a-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="f816a-128">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="f816a-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f816a-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f816a-129">Parent elements</span></span>

|<span data-ttu-id="f816a-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f816a-130">**Element**</span></span>|<span data-ttu-id="f816a-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f816a-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f816a-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="f816a-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="f816a-133">Especifica critérios para os tipos de mensagens a serem encontradas.</span><span class="sxs-lookup"><span data-stu-id="f816a-133">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="f816a-134">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="f816a-134">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="f816a-135">Contém um único resultado de mensagem para um elemento [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="f816a-135">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
|[<span data-ttu-id="f816a-136">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="f816a-136">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="f816a-137">Contém uma única mensagem que é retornada em uma [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="f816a-137">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f816a-138">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="f816a-138">Text value</span></span>

<span data-ttu-id="f816a-139">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f816a-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f816a-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="f816a-140">Remarks</span></span>

<span data-ttu-id="f816a-141">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f816a-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f816a-142">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f816a-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f816a-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="f816a-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f816a-144">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f816a-144">Schema Name</span></span>  <br/> |<span data-ttu-id="f816a-145">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f816a-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="f816a-146">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f816a-146">Validation File</span></span>  <br/> |<span data-ttu-id="f816a-147">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f816a-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f816a-148">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f816a-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="f816a-149">False</span><span class="sxs-lookup"><span data-stu-id="f816a-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f816a-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="f816a-150">See also</span></span>



[<span data-ttu-id="f816a-151">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="f816a-151">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="f816a-152">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f816a-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

