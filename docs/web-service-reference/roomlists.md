---
title: RoomLists
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoomLists
api_type:
- schema
ms.assetid: 2b190823-b11e-4635-97e4-3aba5865fd05
description: O elemento RoomLists é uma lista de um ou mais endereços que representam uma lista de salas de reunião.
ms.openlocfilehash: eb03c34aeb5d80c4a9c6c92471e4094c63f04c87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825252"
---
# <a name="roomlists"></a><span data-ttu-id="695f6-103">RoomLists</span><span class="sxs-lookup"><span data-stu-id="695f6-103">RoomLists</span></span>

<span data-ttu-id="695f6-104">O elemento **RoomLists** é uma lista de um ou mais endereços que representam uma lista de salas de reunião.</span><span class="sxs-lookup"><span data-stu-id="695f6-104">The **RoomLists** element is a list of one or more addresses that represent a list of meeting rooms.</span></span> 
  
[<span data-ttu-id="695f6-105">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="695f6-105">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
  
[<span data-ttu-id="695f6-106">RoomLists</span><span class="sxs-lookup"><span data-stu-id="695f6-106">RoomLists</span></span>](roomlists.md)
  
```xml
<RoomLists>   <Address/></RoomLists>
```

 <span data-ttu-id="695f6-107">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="695f6-107">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="695f6-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="695f6-108">Attributes and elements</span></span>

<span data-ttu-id="695f6-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="695f6-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="695f6-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="695f6-110">Attributes</span></span>

<span data-ttu-id="695f6-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="695f6-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="695f6-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="695f6-112">Child elements</span></span>

|<span data-ttu-id="695f6-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="695f6-113">**Element**</span></span>|<span data-ttu-id="695f6-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="695f6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="695f6-115">Endereço (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="695f6-115">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="695f6-116">Define o endereço de email e o nome de exibição que representa a lista de sala.</span><span class="sxs-lookup"><span data-stu-id="695f6-116">Defines the e-mail address and display name that represents the room list.</span></span> <span data-ttu-id="695f6-117">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="695f6-117">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="695f6-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="695f6-118">Parent elements</span></span>

|<span data-ttu-id="695f6-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="695f6-119">**Element**</span></span>|<span data-ttu-id="695f6-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="695f6-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="695f6-121">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="695f6-121">GetRoomListsResponse</span></span>](getroomlistsresponse.md) <br/> |<span data-ttu-id="695f6-122">Contém o status e o resultado de uma solicitação de [operação GetRoomLists](getroomlists-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="695f6-122">Contains the status and result of a [GetRoomLists operation](getroomlists-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="695f6-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="695f6-123">Remarks</span></span>

<span data-ttu-id="695f6-124">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server com a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="695f6-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="695f6-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="695f6-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="695f6-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="695f6-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="695f6-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="695f6-127">Schema Name</span></span>  <br/> |<span data-ttu-id="695f6-128">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="695f6-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="695f6-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="695f6-129">Validation File</span></span>  <br/> |<span data-ttu-id="695f6-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="695f6-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="695f6-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="695f6-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="695f6-132">False</span><span class="sxs-lookup"><span data-stu-id="695f6-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="695f6-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="695f6-133">See also</span></span>



[<span data-ttu-id="695f6-134">Operação GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="695f6-134">GetRoomLists operation</span></span>](getroomlists-operation.md)


- [<span data-ttu-id="695f6-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="695f6-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

