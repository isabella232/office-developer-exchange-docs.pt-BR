---
title: PlayOnPhone (serviço Web da UM)
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
description: O elemento PlayOnPhone define uma solicitação para reproduzir um item em um telefone.
ms.openlocfilehash: 9acbf9edbf4a889506558b24f5736a44d5015d3f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44434075"
---
# <a name="playonphone-um-web-service"></a><span data-ttu-id="feb1f-103">PlayOnPhone (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="feb1f-103">PlayOnPhone (UM web service)</span></span>

<span data-ttu-id="feb1f-104">O elemento **PlayOnPhone** define uma solicitação para reproduzir um item em um telefone.</span><span class="sxs-lookup"><span data-stu-id="feb1f-104">The **PlayOnPhone** element defines a request to play an item on a telephone.</span></span> 
  
[<span data-ttu-id="feb1f-105">PlayOnPhone (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="feb1f-105">PlayOnPhone (UM web service)</span></span>](playonphone-um-web-service.md)
  
```xml
<PlayOnPhone>
  <entryId>   </entryId>
  <DialString>   </DialString>
</PlayOnPhone>
```

 <span data-ttu-id="feb1f-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="feb1f-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="feb1f-107">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="feb1f-107">Attributes and elements</span></span>

<span data-ttu-id="feb1f-108">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="feb1f-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="feb1f-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="feb1f-109">Attributes</span></span>

<span data-ttu-id="feb1f-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="feb1f-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="feb1f-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="feb1f-111">Child elements</span></span>

|<span data-ttu-id="feb1f-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="feb1f-112">**Element**</span></span>|<span data-ttu-id="feb1f-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="feb1f-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="feb1f-114">EntryID (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="feb1f-114">entryId (UM web service)</span></span>](entryid-um-web-service.md) <br/> |<span data-ttu-id="feb1f-115">Contém o valor que representa o identificador do item a ser tocado no telefone em uma solicitação de [operação do PlayOnPhone (serviço Web da um)](playonphone-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="feb1f-115">Contains the value that represents the identifier of the item to play on the telephone in a [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) request.</span></span>  <br/> |
|[<span data-ttu-id="feb1f-116">dialstring (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="feb1f-116">dialString (UM web service)</span></span>](dialstring-um-web-service.md) <br/> |<span data-ttu-id="feb1f-117">Contém o valor do número de telefone a ser discado.</span><span class="sxs-lookup"><span data-stu-id="feb1f-117">Contains the value for the telephone number to dial.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="feb1f-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="feb1f-118">Parent elements</span></span>

<span data-ttu-id="feb1f-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="feb1f-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="feb1f-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="feb1f-120">Text value</span></span>

<span data-ttu-id="feb1f-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="feb1f-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="feb1f-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="feb1f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="feb1f-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="feb1f-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="feb1f-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="feb1f-124">Schema Name</span></span>  <br/> |<span data-ttu-id="feb1f-125">Mensagens</span><span class="sxs-lookup"><span data-stu-id="feb1f-125">Messages</span></span>  <br/> |
|<span data-ttu-id="feb1f-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="feb1f-126">Validation File</span></span>  <br/> |<span data-ttu-id="feb1f-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="feb1f-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="feb1f-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="feb1f-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="feb1f-129">False</span><span class="sxs-lookup"><span data-stu-id="feb1f-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="feb1f-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="feb1f-130">See also</span></span>



[<span data-ttu-id="feb1f-131">Operação PlayOnPhone (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="feb1f-131">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)

