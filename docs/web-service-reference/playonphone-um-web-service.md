---
title: PlayOnPhone (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 206a2ad1-a01d-4e71-99a1-90c2530423da
description: O elemento de PlayOnPhone define uma solicitação para tocar um item em um telefone.
ms.openlocfilehash: 7e5c1e25512a59d1ac3295b476fcc2b6b0f5a2b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824825"
---
# <a name="playonphone-um-web-service"></a><span data-ttu-id="b8643-103">PlayOnPhone (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="b8643-103">PlayOnPhone (UM web service)</span></span>

<span data-ttu-id="b8643-104">O elemento de **PlayOnPhone** define uma solicitação para tocar um item em um telefone.</span><span class="sxs-lookup"><span data-stu-id="b8643-104">The **PlayOnPhone** element defines a request to play an item on a telephone.</span></span> 
  
[<span data-ttu-id="b8643-105">PlayOnPhone (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="b8643-105">PlayOnPhone (UM web service)</span></span>](playonphone-um-web-service.md)
  
```xml
<PlayOnPhone>
  <entryId>   </entryId>
  <DialString>   </DialString>
</PlayOnPhone>
```

 <span data-ttu-id="b8643-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="b8643-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b8643-107">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b8643-107">Attributes and elements</span></span>

<span data-ttu-id="b8643-108">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b8643-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8643-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="b8643-109">Attributes</span></span>

<span data-ttu-id="b8643-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b8643-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8643-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b8643-111">Child elements</span></span>

|<span data-ttu-id="b8643-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b8643-112">**Element**</span></span>|<span data-ttu-id="b8643-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b8643-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8643-114">entryId (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="b8643-114">entryId (UM web service)</span></span>](entryid-um-web-service.md) <br/> |<span data-ttu-id="b8643-115">Contém o valor que representa o identificador do item para tocar no telefone em uma solicitação de [operação PlayOnPhone (serviço web de Unificação de mensagens)](playonphone-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="b8643-115">Contains the value that represents the identifier of the item to play on the telephone in a [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) request.</span></span>  <br/> |
|[<span data-ttu-id="b8643-116">dialString (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="b8643-116">dialString (UM web service)</span></span>](dialstring-um-web-service.md) <br/> |<span data-ttu-id="b8643-117">Contém o valor para o número de telefone discar.</span><span class="sxs-lookup"><span data-stu-id="b8643-117">Contains the value for the telephone number to dial.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b8643-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b8643-118">Parent elements</span></span>

<span data-ttu-id="b8643-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b8643-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b8643-120">Text value</span><span class="sxs-lookup"><span data-stu-id="b8643-120">Text value</span></span>

<span data-ttu-id="b8643-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b8643-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b8643-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b8643-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b8643-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="b8643-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b8643-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b8643-124">Schema Name</span></span>  <br/> |<span data-ttu-id="b8643-125">Mensagens</span><span class="sxs-lookup"><span data-stu-id="b8643-125">Messages</span></span>  <br/> |
|<span data-ttu-id="b8643-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b8643-126">Validation File</span></span>  <br/> |<span data-ttu-id="b8643-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b8643-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b8643-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b8643-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="b8643-129">False</span><span class="sxs-lookup"><span data-stu-id="b8643-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b8643-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="b8643-130">See also</span></span>



[<span data-ttu-id="b8643-131">Operação de PlayOnPhone (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="b8643-131">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)

