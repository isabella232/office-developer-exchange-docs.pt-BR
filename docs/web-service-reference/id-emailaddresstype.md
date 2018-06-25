---
title: ID (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Id
api_type:
- schema
ms.assetid: 3e1e37b5-5469-4447-ad1f-c2c6d4e0482f
description: O elemento de Id identifica uma sala de reunião dentro da organização do Exchange server.
ms.openlocfilehash: 5cd62f6f4e5912d2ecccda352be15c6a3b24e06c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823847"
---
# <a name="id-emailaddresstype"></a><span data-ttu-id="0aa50-103">ID (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="0aa50-103">Id (EmailAddressType)</span></span>

<span data-ttu-id="0aa50-104">O elemento de **Id** identifica uma sala de reunião dentro da organização do Exchange server.</span><span class="sxs-lookup"><span data-stu-id="0aa50-104">The **Id** element identifies a meeting room within the Exchange server organization.</span></span> 
  
[<span data-ttu-id="0aa50-105">Sala</span><span class="sxs-lookup"><span data-stu-id="0aa50-105">Room</span></span>](room.md)
  
[<span data-ttu-id="0aa50-106">ID (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="0aa50-106">Id (EmailAddressType)</span></span>](id-emailaddresstype.md)
  
```xml
<Id>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Id>
```

 <span data-ttu-id="0aa50-107">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="0aa50-107">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0aa50-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0aa50-108">Attributes and elements</span></span>

<span data-ttu-id="0aa50-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0aa50-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0aa50-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="0aa50-110">Attributes</span></span>

<span data-ttu-id="0aa50-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0aa50-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0aa50-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0aa50-112">Child elements</span></span>

|<span data-ttu-id="0aa50-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0aa50-113">**Element**</span></span>|<span data-ttu-id="0aa50-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0aa50-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0aa50-115">Nome (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="0aa50-115">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="0aa50-116">Define o nome da sala de reunião.</span><span class="sxs-lookup"><span data-stu-id="0aa50-116">Defines the name of the meeting room.</span></span> <span data-ttu-id="0aa50-117">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="0aa50-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="0aa50-118">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="0aa50-118">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="0aa50-119">Define o endereço de Simple Mail Transfer Protocol (SMTP) de uma sala de reunião.</span><span class="sxs-lookup"><span data-stu-id="0aa50-119">Defines the Simple Mail Transfer Protocol (SMTP) address of a meeting room.</span></span> <span data-ttu-id="0aa50-120">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="0aa50-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="0aa50-121">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="0aa50-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="0aa50-122">Define o roteamento que é usado para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0aa50-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="0aa50-123">O padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="0aa50-123">The default is SMTP.</span></span> <span data-ttu-id="0aa50-124">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="0aa50-124">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="0aa50-125">MailboxType</span><span class="sxs-lookup"><span data-stu-id="0aa50-125">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="0aa50-126">Define o tipo de caixa de correio de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0aa50-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="0aa50-127">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="0aa50-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="0aa50-128">ItemId</span><span class="sxs-lookup"><span data-stu-id="0aa50-128">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="0aa50-129">Define o identificador do item de um contato ou uma lista de distribuição particular para destinatários da pasta de contatos do usuário.</span><span class="sxs-lookup"><span data-stu-id="0aa50-129">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="0aa50-130">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="0aa50-130">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0aa50-131">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0aa50-131">Parent elements</span></span>

|<span data-ttu-id="0aa50-132">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0aa50-132">**Element**</span></span>|<span data-ttu-id="0aa50-133">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0aa50-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0aa50-134">Sala</span><span class="sxs-lookup"><span data-stu-id="0aa50-134">Room</span></span>](room.md) <br/> |<span data-ttu-id="0aa50-135">Define uma sala de reunião na organização do Exchange server.</span><span class="sxs-lookup"><span data-stu-id="0aa50-135">Defines a meeting room in the Exchange server organization.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0aa50-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="0aa50-136">Remarks</span></span>

<span data-ttu-id="0aa50-137">O esquema que descreve este elemento está localizado no diretório EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="0aa50-137">The schema that describes this element is located in the EWS directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0aa50-138">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0aa50-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0aa50-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="0aa50-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0aa50-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0aa50-140">Schema Name</span></span>  <br/> |<span data-ttu-id="0aa50-141">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0aa50-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="0aa50-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0aa50-142">Validation File</span></span>  <br/> |<span data-ttu-id="0aa50-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0aa50-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0aa50-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0aa50-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="0aa50-145">False</span><span class="sxs-lookup"><span data-stu-id="0aa50-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0aa50-146">Ver também</span><span class="sxs-lookup"><span data-stu-id="0aa50-146">See also</span></span>



[<span data-ttu-id="0aa50-147">Operação GetRooms</span><span class="sxs-lookup"><span data-stu-id="0aa50-147">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="0aa50-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0aa50-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

