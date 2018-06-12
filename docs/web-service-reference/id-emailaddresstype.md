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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823847"
---
# <a name="id-emailaddresstype"></a><span data-ttu-id="ffba8-103">ID (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ffba8-103">Id (EmailAddressType)</span></span>

<span data-ttu-id="ffba8-104">O elemento de **Id** identifica uma sala de reunião dentro da organização do Exchange server.</span><span class="sxs-lookup"><span data-stu-id="ffba8-104">The **Id** element identifies a meeting room within the Exchange server organization.</span></span> 
  
[<span data-ttu-id="ffba8-105">Sala</span><span class="sxs-lookup"><span data-stu-id="ffba8-105">Room</span></span>](room.md)
  
[<span data-ttu-id="ffba8-106">ID (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ffba8-106">Id (EmailAddressType)</span></span>](id-emailaddresstype.md)
  
```xml
<Id>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Id>
```

 <span data-ttu-id="ffba8-107">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="ffba8-107">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ffba8-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ffba8-108">Attributes and elements</span></span>

<span data-ttu-id="ffba8-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ffba8-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ffba8-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="ffba8-110">Attributes</span></span>

<span data-ttu-id="ffba8-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ffba8-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ffba8-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ffba8-112">Child elements</span></span>

|<span data-ttu-id="ffba8-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ffba8-113">**Element**</span></span>|<span data-ttu-id="ffba8-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ffba8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ffba8-115">Nome (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ffba8-115">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="ffba8-116">Define o nome da sala de reunião.</span><span class="sxs-lookup"><span data-stu-id="ffba8-116">Defines the name of the meeting room.</span></span> <span data-ttu-id="ffba8-117">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="ffba8-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ffba8-118">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="ffba8-118">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="ffba8-119">Define o endereço de Simple Mail Transfer Protocol (SMTP) de uma sala de reunião.</span><span class="sxs-lookup"><span data-stu-id="ffba8-119">Defines the Simple Mail Transfer Protocol (SMTP) address of a meeting room.</span></span> <span data-ttu-id="ffba8-120">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="ffba8-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ffba8-121">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="ffba8-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="ffba8-122">Define o roteamento que é usado para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ffba8-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="ffba8-123">O padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="ffba8-123">The default is SMTP.</span></span> <span data-ttu-id="ffba8-124">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="ffba8-124">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ffba8-125">MailboxType</span><span class="sxs-lookup"><span data-stu-id="ffba8-125">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="ffba8-126">Define o tipo de caixa de correio de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ffba8-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="ffba8-127">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="ffba8-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ffba8-128">ItemId</span><span class="sxs-lookup"><span data-stu-id="ffba8-128">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ffba8-129">Define o identificador do item de um contato ou uma lista de distribuição particular para destinatários da pasta de contatos do usuário.</span><span class="sxs-lookup"><span data-stu-id="ffba8-129">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="ffba8-130">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="ffba8-130">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ffba8-131">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ffba8-131">Parent elements</span></span>

|<span data-ttu-id="ffba8-132">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ffba8-132">**Element**</span></span>|<span data-ttu-id="ffba8-133">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ffba8-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ffba8-134">Sala</span><span class="sxs-lookup"><span data-stu-id="ffba8-134">Room</span></span>](room.md) <br/> |<span data-ttu-id="ffba8-135">Define uma sala de reunião na organização do Exchange server.</span><span class="sxs-lookup"><span data-stu-id="ffba8-135">Defines a meeting room in the Exchange server organization.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ffba8-136">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="ffba8-136">Remarks</span></span>

<span data-ttu-id="ffba8-137">O esquema que descreve este elemento está localizado no diretório EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="ffba8-137">The schema that describes this element is located in the EWS directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ffba8-138">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ffba8-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ffba8-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="ffba8-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ffba8-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ffba8-140">Schema Name</span></span>  <br/> |<span data-ttu-id="ffba8-141">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ffba8-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="ffba8-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ffba8-142">Validation File</span></span>  <br/> |<span data-ttu-id="ffba8-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ffba8-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ffba8-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ffba8-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="ffba8-145">False</span><span class="sxs-lookup"><span data-stu-id="ffba8-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ffba8-146">Ver também</span><span class="sxs-lookup"><span data-stu-id="ffba8-146">See also</span></span>



[<span data-ttu-id="ffba8-147">Operação GetRooms</span><span class="sxs-lookup"><span data-stu-id="ffba8-147">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="ffba8-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ffba8-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

