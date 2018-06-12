---
title: GetRooms
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRooms
api_type:
- schema
ms.assetid: 82a737c7-da41-4777-8ad8-89851a0b602b
description: O GetRooms é o elemento raiz em uma solicitação para obter uma lista de salas dentro de uma lista de salas específico.
ms.openlocfilehash: a787097752cfeee9489e5f118549c2d939ba4c9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752619"
---
# <a name="getrooms"></a><span data-ttu-id="7449f-103">GetRooms</span><span class="sxs-lookup"><span data-stu-id="7449f-103">GetRooms</span></span>

<span data-ttu-id="7449f-104">O **GetRooms** é o elemento raiz em uma solicitação para obter uma lista de salas dentro de uma lista de salas específico.</span><span class="sxs-lookup"><span data-stu-id="7449f-104">The **GetRooms** element is the root element in a request to get a list of rooms within a particular room list.</span></span> 
  
```XML
<GetRooms>
   <RoomList/>
</GetRooms>
```

 <span data-ttu-id="7449f-105">**GetRoomsType**</span><span class="sxs-lookup"><span data-stu-id="7449f-105">**GetRoomsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7449f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7449f-106">Attributes and elements</span></span>

<span data-ttu-id="7449f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7449f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7449f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7449f-108">Attributes</span></span>

<span data-ttu-id="7449f-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7449f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7449f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7449f-110">Child elements</span></span>

|<span data-ttu-id="7449f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7449f-111">**Element**</span></span>|<span data-ttu-id="7449f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7449f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7449f-113">RoomList</span><span class="sxs-lookup"><span data-stu-id="7449f-113">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="7449f-114">Representa um endereço de email que identifica uma lista de salas de reunião</span><span class="sxs-lookup"><span data-stu-id="7449f-114">Represents an e-mail address that identifies a list of meeting rooms</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7449f-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7449f-115">Parent elements</span></span>

<span data-ttu-id="7449f-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7449f-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="7449f-117">Text value</span><span class="sxs-lookup"><span data-stu-id="7449f-117">Text value</span></span>

<span data-ttu-id="7449f-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7449f-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7449f-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="7449f-119">Remarks</span></span>

<span data-ttu-id="7449f-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7449f-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7449f-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7449f-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7449f-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="7449f-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7449f-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7449f-123">Schema Name</span></span>  <br/> |<span data-ttu-id="7449f-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="7449f-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7449f-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7449f-125">Validation File</span></span>  <br/> |<span data-ttu-id="7449f-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7449f-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7449f-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7449f-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="7449f-128">False</span><span class="sxs-lookup"><span data-stu-id="7449f-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7449f-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="7449f-129">See also</span></span>



- [<span data-ttu-id="7449f-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7449f-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

