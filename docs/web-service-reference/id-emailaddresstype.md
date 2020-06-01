---
title: ID (EmailAddresstype)
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
description: O elemento ID identifica uma sala de reunião na organização do Exchange Server.
ms.openlocfilehash: aa09e7764746ac6bc283de2d13248d769aba75b7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460775"
---
# <a name="id-emailaddresstype"></a><span data-ttu-id="d34b4-103">ID (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="d34b4-103">Id (EmailAddressType)</span></span>

<span data-ttu-id="d34b4-104">O elemento **ID** identifica uma sala de reunião na organização do Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="d34b4-104">The **Id** element identifies a meeting room within the Exchange server organization.</span></span> 
  
[<span data-ttu-id="d34b4-105">Sala</span><span class="sxs-lookup"><span data-stu-id="d34b4-105">Room</span></span>](room.md)
  
[<span data-ttu-id="d34b4-106">ID (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="d34b4-106">Id (EmailAddressType)</span></span>](id-emailaddresstype.md)
  
```xml
<Id>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Id>
```

 <span data-ttu-id="d34b4-107">**EmailAddresstype**</span><span class="sxs-lookup"><span data-stu-id="d34b4-107">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d34b4-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d34b4-108">Attributes and elements</span></span>

<span data-ttu-id="d34b4-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d34b4-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d34b4-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="d34b4-110">Attributes</span></span>

<span data-ttu-id="d34b4-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d34b4-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d34b4-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d34b4-112">Child elements</span></span>

|<span data-ttu-id="d34b4-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d34b4-113">**Element**</span></span>|<span data-ttu-id="d34b4-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d34b4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d34b4-115">Nome (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="d34b4-115">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="d34b4-116">Define o nome da sala de reunião.</span><span class="sxs-lookup"><span data-stu-id="d34b4-116">Defines the name of the meeting room.</span></span> <span data-ttu-id="d34b4-117">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="d34b4-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d34b4-118">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="d34b4-118">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="d34b4-119">Define o endereço SMTP (Simple Mail Transfer Protocol) de uma sala de reunião.</span><span class="sxs-lookup"><span data-stu-id="d34b4-119">Defines the Simple Mail Transfer Protocol (SMTP) address of a meeting room.</span></span> <span data-ttu-id="d34b4-120">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="d34b4-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d34b4-121">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="d34b4-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="d34b4-122">Define o roteamento usado para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d34b4-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="d34b4-123">O padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="d34b4-123">The default is SMTP.</span></span> <span data-ttu-id="d34b4-124">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="d34b4-124">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d34b4-125">MailboxType</span><span class="sxs-lookup"><span data-stu-id="d34b4-125">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="d34b4-126">Define o tipo de caixa de correio de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d34b4-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="d34b4-127">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="d34b4-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d34b4-128">ItemId</span><span class="sxs-lookup"><span data-stu-id="d34b4-128">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="d34b4-129">Define o identificador de item de um contato ou de uma lista de distribuição privada para destinatários da pasta contatos de um usuário.</span><span class="sxs-lookup"><span data-stu-id="d34b4-129">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="d34b4-130">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="d34b4-130">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d34b4-131">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d34b4-131">Parent elements</span></span>

|<span data-ttu-id="d34b4-132">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d34b4-132">**Element**</span></span>|<span data-ttu-id="d34b4-133">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d34b4-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d34b4-134">Sala</span><span class="sxs-lookup"><span data-stu-id="d34b4-134">Room</span></span>](room.md) <br/> |<span data-ttu-id="d34b4-135">Define uma sala de reunião na organização do Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="d34b4-135">Defines a meeting room in the Exchange server organization.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d34b4-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="d34b4-136">Remarks</span></span>

<span data-ttu-id="d34b4-137">O esquema que descreve este elemento está localizado no diretório do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="d34b4-137">The schema that describes this element is located in the EWS directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d34b4-138">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d34b4-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d34b4-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="d34b4-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d34b4-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d34b4-140">Schema Name</span></span>  <br/> |<span data-ttu-id="d34b4-141">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d34b4-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="d34b4-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d34b4-142">Validation File</span></span>  <br/> |<span data-ttu-id="d34b4-143">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d34b4-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d34b4-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d34b4-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="d34b4-145">False</span><span class="sxs-lookup"><span data-stu-id="d34b4-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d34b4-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="d34b4-146">See also</span></span>



[<span data-ttu-id="d34b4-147">Operação getrooms</span><span class="sxs-lookup"><span data-stu-id="d34b4-147">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="d34b4-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d34b4-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

