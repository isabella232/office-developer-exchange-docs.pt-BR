---
title: Getrooms
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
description: O elemento getrooms é o elemento raiz em uma solicitação para obter uma lista de salas em uma determinada lista de salas.
ms.openlocfilehash: 77fde5980a03d4c0509344933b0901cb21ab7197
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458590"
---
# <a name="getrooms"></a><span data-ttu-id="9edaf-103">Getrooms</span><span class="sxs-lookup"><span data-stu-id="9edaf-103">GetRooms</span></span>

<span data-ttu-id="9edaf-104">O elemento **Getrooms** é o elemento raiz em uma solicitação para obter uma lista de salas em uma determinada lista de salas.</span><span class="sxs-lookup"><span data-stu-id="9edaf-104">The **GetRooms** element is the root element in a request to get a list of rooms within a particular room list.</span></span> 
  
```XML
<GetRooms>
   <RoomList/>
</GetRooms>
```

 <span data-ttu-id="9edaf-105">**Getroomtype**</span><span class="sxs-lookup"><span data-stu-id="9edaf-105">**GetRoomsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9edaf-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9edaf-106">Attributes and elements</span></span>

<span data-ttu-id="9edaf-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9edaf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9edaf-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9edaf-108">Attributes</span></span>

<span data-ttu-id="9edaf-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9edaf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9edaf-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9edaf-110">Child elements</span></span>

|<span data-ttu-id="9edaf-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9edaf-111">**Element**</span></span>|<span data-ttu-id="9edaf-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9edaf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9edaf-113">RoomList</span><span class="sxs-lookup"><span data-stu-id="9edaf-113">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="9edaf-114">Representa um endereço de email que identifica uma lista de salas de reunião</span><span class="sxs-lookup"><span data-stu-id="9edaf-114">Represents an e-mail address that identifies a list of meeting rooms</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9edaf-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9edaf-115">Parent elements</span></span>

<span data-ttu-id="9edaf-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9edaf-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="9edaf-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="9edaf-117">Text value</span></span>

<span data-ttu-id="9edaf-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9edaf-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9edaf-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="9edaf-119">Remarks</span></span>

<span data-ttu-id="9edaf-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9edaf-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9edaf-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9edaf-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9edaf-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="9edaf-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9edaf-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9edaf-123">Schema Name</span></span>  <br/> |<span data-ttu-id="9edaf-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="9edaf-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9edaf-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9edaf-125">Validation File</span></span>  <br/> |<span data-ttu-id="9edaf-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9edaf-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9edaf-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9edaf-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="9edaf-128">False</span><span class="sxs-lookup"><span data-stu-id="9edaf-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9edaf-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="9edaf-129">See also</span></span>



- [<span data-ttu-id="9edaf-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9edaf-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

