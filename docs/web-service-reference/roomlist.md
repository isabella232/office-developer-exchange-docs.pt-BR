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
ms.openlocfilehash: 0444475cb9fffbb89ba2861096baee0c7e645995
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460516"
---
# <a name="roomlist"></a><span data-ttu-id="db568-103">RoomList</span><span class="sxs-lookup"><span data-stu-id="db568-103">RoomList</span></span>

<span data-ttu-id="db568-104">O elemento **RoomList** representa um endereço de email que identifica uma lista de salas de reunião.</span><span class="sxs-lookup"><span data-stu-id="db568-104">The **RoomList** element represents an e-mail address that identifies a list of meeting rooms.</span></span> 
  
[<span data-ttu-id="db568-105">Getrooms</span><span class="sxs-lookup"><span data-stu-id="db568-105">GetRooms</span></span>](getrooms.md)
  
[<span data-ttu-id="db568-106">RoomList</span><span class="sxs-lookup"><span data-stu-id="db568-106">RoomList</span></span>](roomlist.md)
  
```XML
<RoomList>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RoomList>
```

 <span data-ttu-id="db568-107">**EmailAddresstype**</span><span class="sxs-lookup"><span data-stu-id="db568-107">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="db568-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="db568-108">Attributes and elements</span></span>

<span data-ttu-id="db568-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="db568-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db568-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="db568-110">Attributes</span></span>

<span data-ttu-id="db568-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="db568-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="db568-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="db568-112">Child elements</span></span>

|<span data-ttu-id="db568-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="db568-113">**Element**</span></span>|<span data-ttu-id="db568-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="db568-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db568-115">Nome (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="db568-115">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="db568-116">Define o nome de exibição da lista de salas.</span><span class="sxs-lookup"><span data-stu-id="db568-116">Defines the display name of the room list.</span></span> <span data-ttu-id="db568-117">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="db568-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="db568-118">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="db568-118">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="db568-119">Define o endereço SMTP (Simple Mail Transfer Protocol) de uma lista de salas.</span><span class="sxs-lookup"><span data-stu-id="db568-119">Defines the Simple Mail Transfer Protocol (SMTP) address of a room list.</span></span> <span data-ttu-id="db568-120">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="db568-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="db568-121">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="db568-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="db568-122">Define o roteamento usado para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="db568-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="db568-123">O padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="db568-123">The default is SMTP.</span></span> <span data-ttu-id="db568-124">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="db568-124">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="db568-125">MailboxType</span><span class="sxs-lookup"><span data-stu-id="db568-125">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="db568-126">Define o tipo de caixa de correio de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="db568-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="db568-127">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="db568-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="db568-128">ItemId</span><span class="sxs-lookup"><span data-stu-id="db568-128">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="db568-129">Define o identificador de item de um contato ou de uma lista de distribuição privada para destinatários da pasta contatos de um usuário.</span><span class="sxs-lookup"><span data-stu-id="db568-129">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="db568-130">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="db568-130">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="db568-131">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="db568-131">Parent elements</span></span>

|<span data-ttu-id="db568-132">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="db568-132">**Element**</span></span>|<span data-ttu-id="db568-133">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="db568-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db568-134">Getrooms</span><span class="sxs-lookup"><span data-stu-id="db568-134">GetRooms</span></span>](getrooms.md) <br/> |<span data-ttu-id="db568-135">O elemento raiz em uma solicitação para obter uma lista de salas dentro de uma determinada lista de salas.</span><span class="sxs-lookup"><span data-stu-id="db568-135">The root element in a request to get a list of rooms within a particular room list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="db568-136">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="db568-136">Text value</span></span>

<span data-ttu-id="db568-137">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="db568-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="db568-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="db568-138">Remarks</span></span>

<span data-ttu-id="db568-139">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="db568-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="db568-140">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="db568-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db568-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="db568-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="db568-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="db568-142">Schema Name</span></span>  <br/> |<span data-ttu-id="db568-143">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="db568-143">Messages schema</span></span>  <br/> |
|<span data-ttu-id="db568-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="db568-144">Validation File</span></span>  <br/> |<span data-ttu-id="db568-145">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="db568-145">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="db568-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="db568-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="db568-147">False</span><span class="sxs-lookup"><span data-stu-id="db568-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="db568-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="db568-148">See also</span></span>



[<span data-ttu-id="db568-149">Operação getrooms</span><span class="sxs-lookup"><span data-stu-id="db568-149">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="db568-150">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="db568-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

