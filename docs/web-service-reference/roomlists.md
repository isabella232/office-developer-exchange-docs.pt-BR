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
ms.openlocfilehash: 8f6393b617331e5878e48113c94ca3546cba095e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459045"
---
# <a name="roomlists"></a><span data-ttu-id="dca6c-103">RoomLists</span><span class="sxs-lookup"><span data-stu-id="dca6c-103">RoomLists</span></span>

<span data-ttu-id="dca6c-104">O elemento **RoomLists** é uma lista de um ou mais endereços que representam uma lista de salas de reunião.</span><span class="sxs-lookup"><span data-stu-id="dca6c-104">The **RoomLists** element is a list of one or more addresses that represent a list of meeting rooms.</span></span> 
  
[<span data-ttu-id="dca6c-105">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="dca6c-105">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
  
[<span data-ttu-id="dca6c-106">RoomLists</span><span class="sxs-lookup"><span data-stu-id="dca6c-106">RoomLists</span></span>](roomlists.md)
  
```xml
<RoomLists>   <Address/></RoomLists>
```

 <span data-ttu-id="dca6c-107">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="dca6c-107">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dca6c-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="dca6c-108">Attributes and elements</span></span>

<span data-ttu-id="dca6c-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="dca6c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dca6c-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="dca6c-110">Attributes</span></span>

<span data-ttu-id="dca6c-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dca6c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dca6c-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="dca6c-112">Child elements</span></span>

|<span data-ttu-id="dca6c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dca6c-113">**Element**</span></span>|<span data-ttu-id="dca6c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dca6c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dca6c-115">Endereço (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="dca6c-115">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="dca6c-116">Define o endereço de email e o nome de exibição que representa a lista de salas.</span><span class="sxs-lookup"><span data-stu-id="dca6c-116">Defines the e-mail address and display name that represents the room list.</span></span> <span data-ttu-id="dca6c-117">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="dca6c-117">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dca6c-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="dca6c-118">Parent elements</span></span>

|<span data-ttu-id="dca6c-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dca6c-119">**Element**</span></span>|<span data-ttu-id="dca6c-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dca6c-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dca6c-121">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="dca6c-121">GetRoomListsResponse</span></span>](getroomlistsresponse.md) <br/> |<span data-ttu-id="dca6c-122">Contém o status e o resultado de uma solicitação de [operação GetRoomLists](getroomlists-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dca6c-122">Contains the status and result of a [GetRoomLists operation](getroomlists-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dca6c-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="dca6c-123">Remarks</span></span>

<span data-ttu-id="dca6c-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Exchange Server com a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="dca6c-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dca6c-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="dca6c-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dca6c-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="dca6c-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dca6c-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="dca6c-127">Schema Name</span></span>  <br/> |<span data-ttu-id="dca6c-128">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="dca6c-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dca6c-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="dca6c-129">Validation File</span></span>  <br/> |<span data-ttu-id="dca6c-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dca6c-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dca6c-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="dca6c-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="dca6c-132">False</span><span class="sxs-lookup"><span data-stu-id="dca6c-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dca6c-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="dca6c-133">See also</span></span>



[<span data-ttu-id="dca6c-134">Operação GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="dca6c-134">GetRoomLists operation</span></span>](getroomlists-operation.md)


- [<span data-ttu-id="dca6c-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="dca6c-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

