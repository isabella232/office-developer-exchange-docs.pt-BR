---
title: ReturnQueueEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReturnQueueEvents
api_type:
- schema
ms.assetid: 69d22417-320c-4c6f-9fb4-2020f2480bb2
description: O elemento ReturnQueueEvents indica que a pessoa que está executando a tarefa está em uma função privilegiada.
ms.openlocfilehash: 02f4ca86ffa14117105ec186ae039065cb626670
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825233"
---
# <a name="returnqueueevents"></a><span data-ttu-id="3e918-103">ReturnQueueEvents</span><span class="sxs-lookup"><span data-stu-id="3e918-103">ReturnQueueEvents</span></span>

<span data-ttu-id="3e918-104">O elemento **ReturnQueueEvents** indica que a pessoa que está executando a tarefa está em uma função privilegiada.</span><span class="sxs-lookup"><span data-stu-id="3e918-104">The **ReturnQueueEvents** element indicates that the person who is running the task is in a privileged role.</span></span> 
  
```XML
<ReturnQueueEvents>true | false</ReturnQueueEvents>
```

 <span data-ttu-id="3e918-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3e918-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3e918-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3e918-106">Attributes and elements</span></span>

<span data-ttu-id="3e918-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3e918-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3e918-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3e918-108">Attributes</span></span>

<span data-ttu-id="3e918-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3e918-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3e918-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3e918-110">Child elements</span></span>

<span data-ttu-id="3e918-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3e918-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3e918-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3e918-112">Parent elements</span></span>

|<span data-ttu-id="3e918-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3e918-113">**Element**</span></span>|<span data-ttu-id="3e918-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3e918-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e918-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="3e918-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="3e918-116">Contém a solicitação para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) recuperar a mensagem completa relatório de rastreamento para a ID especificada.</span><span class="sxs-lookup"><span data-stu-id="3e918-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3e918-117">Text value</span><span class="sxs-lookup"><span data-stu-id="3e918-117">Text value</span></span>

<span data-ttu-id="3e918-118">É necessário um valor de texto que representa um valor booleano.</span><span class="sxs-lookup"><span data-stu-id="3e918-118">A text value that represents a Boolean value is required.</span></span> <span data-ttu-id="3e918-119">Um valor **true** indica que a pessoa que está executando a tarefa está em uma função privilegiada; um valor **false** indica que a pessoa que está executando a tarefa não está em uma função privilegiada.</span><span class="sxs-lookup"><span data-stu-id="3e918-119">A value of **true** indicates that the person who is running the task is in a privileged role; a value of **false** indicates that the person who is running the task is not in a privileged role.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3e918-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="3e918-120">Remarks</span></span>

<span data-ttu-id="3e918-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e918-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3e918-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3e918-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3e918-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="3e918-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3e918-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3e918-124">Schema Name</span></span>  <br/> |<span data-ttu-id="3e918-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="3e918-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3e918-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3e918-126">Validation File</span></span>  <br/> |<span data-ttu-id="3e918-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3e918-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3e918-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3e918-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="3e918-129">False</span><span class="sxs-lookup"><span data-stu-id="3e918-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3e918-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="3e918-130">See also</span></span>



[<span data-ttu-id="3e918-131">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="3e918-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="3e918-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3e918-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

