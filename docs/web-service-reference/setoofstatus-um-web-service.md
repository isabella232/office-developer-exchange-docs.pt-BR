---
title: SetOofStatus (serviço Web da UM)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetOofStatus
api_type:
- schema
ms.assetid: 9fc0ea9c-7a98-4fd7-a90c-cf5639c63a3a
description: O elemento SetOofStatus define uma solicitação para definir o status de ausência temporária da Unificação de mensagens do Office (OOF) para o usuário que faz a solicitação.
ms.openlocfilehash: 86e056a440e282cd444cfd405e452720b26b7456
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467064"
---
# <a name="setoofstatus-um-web-service"></a><span data-ttu-id="7586c-103">SetOofStatus (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="7586c-103">SetOofStatus (UM web service)</span></span>

<span data-ttu-id="7586c-104">O elemento **SetOofStatus** define uma solicitação para definir o status de ausência temporária da Unificação de mensagens do Office (OOF) para o usuário que faz a solicitação.</span><span class="sxs-lookup"><span data-stu-id="7586c-104">The **SetOofStatus** element defines a request to set the Unified Messaging Out of Office (OOF) status for the user who makes the request.</span></span> 
  
[<span data-ttu-id="7586c-105">SetOofStatus (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="7586c-105">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md)
  
```xml
<SetOofStatus>
  <status/>
</SetOofStatus>
```

 <span data-ttu-id="7586c-106">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="7586c-106">**Type**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7586c-107">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="7586c-107">Attributes and elements</span></span>

<span data-ttu-id="7586c-108">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7586c-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7586c-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="7586c-109">Attributes</span></span>

<span data-ttu-id="7586c-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7586c-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7586c-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7586c-111">Child elements</span></span>

|<span data-ttu-id="7586c-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7586c-112">**Element**</span></span>|<span data-ttu-id="7586c-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7586c-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7586c-114">Status (serviço Web da UM-SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="7586c-114">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md) <br/> |<span data-ttu-id="7586c-115">Define um valor a ser usado em uma solicitação de [operação do SetOofStatus (serviço Web da um)](setoofstatus-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="7586c-115">Defines a value to use in a [SetOofStatus operation (UM web service)](setoofstatus-operation-um-web-service.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7586c-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7586c-116">Parent elements</span></span>

<span data-ttu-id="7586c-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7586c-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="7586c-118">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="7586c-118">Text value</span></span>

<span data-ttu-id="7586c-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7586c-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7586c-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="7586c-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7586c-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="7586c-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7586c-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7586c-122">Schema Name</span></span>  <br/> |<span data-ttu-id="7586c-123">Mensagens</span><span class="sxs-lookup"><span data-stu-id="7586c-123">Messages</span></span>  <br/> |
|<span data-ttu-id="7586c-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7586c-124">Validation File</span></span>  <br/> |<span data-ttu-id="7586c-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7586c-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7586c-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7586c-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="7586c-127">False</span><span class="sxs-lookup"><span data-stu-id="7586c-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7586c-128">Confira também</span><span class="sxs-lookup"><span data-stu-id="7586c-128">See also</span></span>



[<span data-ttu-id="7586c-129">Operação SetOofStatus (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="7586c-129">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)
  
[<span data-ttu-id="7586c-130">Status (serviço Web da UM-SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="7586c-130">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md)

