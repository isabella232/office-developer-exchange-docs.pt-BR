---
title: Quartos
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
description: O elemento Rooms é uma lista de um ou mais elementos que representam salas de reunião.
ms.openlocfilehash: f8b60a9680f6abba459ebecc96613abfdd93766d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466182"
---
# <a name="rooms"></a><span data-ttu-id="fbc68-103">Quartos</span><span class="sxs-lookup"><span data-stu-id="fbc68-103">Rooms</span></span>

<span data-ttu-id="fbc68-104">O elemento **Rooms** é uma lista de um ou mais elementos que representam salas de reunião.</span><span class="sxs-lookup"><span data-stu-id="fbc68-104">The **Rooms** element is a list of one or more elements that represent meeting rooms.</span></span> 
  
[<span data-ttu-id="fbc68-105">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="fbc68-105">GetRoomsResponse</span></span>](getroomsresponse.md)
  
[<span data-ttu-id="fbc68-106">Quartos</span><span class="sxs-lookup"><span data-stu-id="fbc68-106">Rooms</span></span>](rooms.md)
  
```xml
<Rooms>   <Room/></Rooms>
```

 <span data-ttu-id="fbc68-107">**ArrayOfRoomsType**</span><span class="sxs-lookup"><span data-stu-id="fbc68-107">**ArrayOfRoomsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fbc68-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fbc68-108">Attributes and elements</span></span>

<span data-ttu-id="fbc68-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fbc68-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fbc68-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="fbc68-110">Attributes</span></span>

<span data-ttu-id="fbc68-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fbc68-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fbc68-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fbc68-112">Child elements</span></span>

|<span data-ttu-id="fbc68-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fbc68-113">**Element**</span></span>|<span data-ttu-id="fbc68-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fbc68-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fbc68-115">Sala</span><span class="sxs-lookup"><span data-stu-id="fbc68-115">Room</span></span>](room.md) <br/> |<span data-ttu-id="fbc68-116">Define um endereço de email e um nome para exibição que representa uma sala de reunião.</span><span class="sxs-lookup"><span data-stu-id="fbc68-116">Defines an e-mail address and display name that represents a meeting room.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fbc68-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fbc68-117">Parent elements</span></span>

|<span data-ttu-id="fbc68-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fbc68-118">**Element**</span></span>|<span data-ttu-id="fbc68-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fbc68-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fbc68-120">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="fbc68-120">GetRoomsResponse</span></span>](getroomsresponse.md) <br/> ||
   
## <a name="remarks"></a><span data-ttu-id="fbc68-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="fbc68-121">Remarks</span></span>

<span data-ttu-id="fbc68-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="fbc68-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fbc68-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="fbc68-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fbc68-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="fbc68-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fbc68-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fbc68-125">Schema Name</span></span>  <br/> |<span data-ttu-id="fbc68-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="fbc68-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fbc68-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fbc68-127">Validation File</span></span>  <br/> |<span data-ttu-id="fbc68-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fbc68-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fbc68-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fbc68-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="fbc68-130">False</span><span class="sxs-lookup"><span data-stu-id="fbc68-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fbc68-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="fbc68-131">See also</span></span>



[<span data-ttu-id="fbc68-132">Operação getrooms</span><span class="sxs-lookup"><span data-stu-id="fbc68-132">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="fbc68-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fbc68-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

