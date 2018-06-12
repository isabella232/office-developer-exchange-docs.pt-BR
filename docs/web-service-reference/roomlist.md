---
title: RoomList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoomList
api_type:
- schema
ms.assetid: cb02bdf0-df9f-4e31-b7dd-cd9f2f2cc2b2
description: O elemento RoomList representa um endereço de email que identifica uma lista de salas de reunião.
ms.openlocfilehash: 7de2c67f8001387abf463186933f0b81ee45a58a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825262"
---
# <a name="roomlist"></a><span data-ttu-id="95206-103">RoomList</span><span class="sxs-lookup"><span data-stu-id="95206-103">RoomList</span></span>

<span data-ttu-id="95206-104">O elemento **RoomList** representa um endereço de email que identifica uma lista de salas de reunião.</span><span class="sxs-lookup"><span data-stu-id="95206-104">The **RoomList** element represents an e-mail address that identifies a list of meeting rooms.</span></span> 
  
[<span data-ttu-id="95206-105">GetRooms</span><span class="sxs-lookup"><span data-stu-id="95206-105">GetRooms</span></span>](getrooms.md)
  
[<span data-ttu-id="95206-106">RoomList</span><span class="sxs-lookup"><span data-stu-id="95206-106">RoomList</span></span>](roomlist.md)
  
```XML
<RoomList>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RoomList>
```

 <span data-ttu-id="95206-107">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="95206-107">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="95206-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="95206-108">Attributes and elements</span></span>

<span data-ttu-id="95206-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="95206-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="95206-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="95206-110">Attributes</span></span>

<span data-ttu-id="95206-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="95206-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="95206-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="95206-112">Child elements</span></span>

|<span data-ttu-id="95206-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="95206-113">**Element**</span></span>|<span data-ttu-id="95206-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="95206-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95206-115">Nome (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="95206-115">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="95206-116">Define o nome de exibição da lista de sala.</span><span class="sxs-lookup"><span data-stu-id="95206-116">Defines the display name of the room list.</span></span> <span data-ttu-id="95206-117">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="95206-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="95206-118">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="95206-118">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="95206-119">Define o endereço de Simple Mail Transfer Protocol (SMTP) de uma lista de salas.</span><span class="sxs-lookup"><span data-stu-id="95206-119">Defines the Simple Mail Transfer Protocol (SMTP) address of a room list.</span></span> <span data-ttu-id="95206-120">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="95206-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="95206-121">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="95206-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="95206-122">Define o roteamento que é usado para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="95206-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="95206-123">O padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="95206-123">The default is SMTP.</span></span> <span data-ttu-id="95206-124">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="95206-124">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="95206-125">MailboxType</span><span class="sxs-lookup"><span data-stu-id="95206-125">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="95206-126">Define o tipo de caixa de correio de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="95206-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="95206-127">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="95206-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="95206-128">ItemId</span><span class="sxs-lookup"><span data-stu-id="95206-128">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="95206-129">Define o identificador do item de um contato ou uma lista de distribuição particular para destinatários da pasta de contatos do usuário.</span><span class="sxs-lookup"><span data-stu-id="95206-129">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="95206-130">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="95206-130">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="95206-131">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="95206-131">Parent elements</span></span>

|<span data-ttu-id="95206-132">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="95206-132">**Element**</span></span>|<span data-ttu-id="95206-133">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="95206-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95206-134">GetRooms</span><span class="sxs-lookup"><span data-stu-id="95206-134">GetRooms</span></span>](getrooms.md) <br/> |<span data-ttu-id="95206-135">O elemento raiz em uma solicitação para obter uma lista de salas dentro de uma lista de salas específico.</span><span class="sxs-lookup"><span data-stu-id="95206-135">The root element in a request to get a list of rooms within a particular room list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="95206-136">Text value</span><span class="sxs-lookup"><span data-stu-id="95206-136">Text value</span></span>

<span data-ttu-id="95206-137">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="95206-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="95206-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="95206-138">Remarks</span></span>

<span data-ttu-id="95206-139">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="95206-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="95206-140">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="95206-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="95206-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="95206-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="95206-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="95206-142">Schema Name</span></span>  <br/> |<span data-ttu-id="95206-143">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="95206-143">Messages schema</span></span>  <br/> |
|<span data-ttu-id="95206-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="95206-144">Validation File</span></span>  <br/> |<span data-ttu-id="95206-145">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="95206-145">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="95206-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="95206-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="95206-147">False</span><span class="sxs-lookup"><span data-stu-id="95206-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="95206-148">Ver também</span><span class="sxs-lookup"><span data-stu-id="95206-148">See also</span></span>



[<span data-ttu-id="95206-149">Operação GetRooms</span><span class="sxs-lookup"><span data-stu-id="95206-149">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="95206-150">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="95206-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

