---
title: Salas
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rooms
api_type:
- schema
ms.assetid: 57b6079a-3d83-4429-861e-c551e9e1a991
description: O elemento de salas é uma lista de um ou mais elementos que representam as salas de reunião.
ms.openlocfilehash: e95112d3d565da29c309e45710ffc0ea9b4d5064
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825249"
---
# <a name="rooms"></a><span data-ttu-id="cf926-103">Salas</span><span class="sxs-lookup"><span data-stu-id="cf926-103">Rooms</span></span>

<span data-ttu-id="cf926-104">O elemento de **salas** é uma lista de um ou mais elementos que representam as salas de reunião.</span><span class="sxs-lookup"><span data-stu-id="cf926-104">The **Rooms** element is a list of one or more elements that represent meeting rooms.</span></span> 
  
[<span data-ttu-id="cf926-105">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="cf926-105">GetRoomsResponse</span></span>](getroomsresponse.md)
  
[<span data-ttu-id="cf926-106">Salas</span><span class="sxs-lookup"><span data-stu-id="cf926-106">Rooms</span></span>](rooms.md)
  
```xml
<Rooms>   <Room/></Rooms>
```

 <span data-ttu-id="cf926-107">**ArrayOfRoomsType**</span><span class="sxs-lookup"><span data-stu-id="cf926-107">**ArrayOfRoomsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf926-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="cf926-108">Attributes and elements</span></span>

<span data-ttu-id="cf926-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cf926-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf926-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="cf926-110">Attributes</span></span>

<span data-ttu-id="cf926-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cf926-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf926-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cf926-112">Child elements</span></span>

|<span data-ttu-id="cf926-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cf926-113">**Element**</span></span>|<span data-ttu-id="cf926-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cf926-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf926-115">Sala</span><span class="sxs-lookup"><span data-stu-id="cf926-115">Room</span></span>](room.md) <br/> |<span data-ttu-id="cf926-116">Define um endereço de email e o nome de exibição que representa uma sala de reunião.</span><span class="sxs-lookup"><span data-stu-id="cf926-116">Defines an e-mail address and display name that represents a meeting room.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cf926-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cf926-117">Parent elements</span></span>

|<span data-ttu-id="cf926-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cf926-118">**Element**</span></span>|<span data-ttu-id="cf926-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cf926-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf926-120">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="cf926-120">GetRoomsResponse</span></span>](getroomsresponse.md) <br/> ||
   
## <a name="remarks"></a><span data-ttu-id="cf926-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="cf926-121">Remarks</span></span>

<span data-ttu-id="cf926-122">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="cf926-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf926-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="cf926-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf926-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="cf926-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cf926-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cf926-125">Schema Name</span></span>  <br/> |<span data-ttu-id="cf926-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="cf926-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cf926-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cf926-127">Validation File</span></span>  <br/> |<span data-ttu-id="cf926-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cf926-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cf926-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cf926-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf926-130">False</span><span class="sxs-lookup"><span data-stu-id="cf926-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf926-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="cf926-131">See also</span></span>



[<span data-ttu-id="cf926-132">Operação GetRooms</span><span class="sxs-lookup"><span data-stu-id="cf926-132">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="cf926-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cf926-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

