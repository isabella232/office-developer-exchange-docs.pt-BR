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
ms.openlocfilehash: 9d07bc8c3d32f1cd532febaf4ae04e4a2d31d243
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466588"
---
# <a name="returnqueueevents"></a><span data-ttu-id="11ae3-103">ReturnQueueEvents</span><span class="sxs-lookup"><span data-stu-id="11ae3-103">ReturnQueueEvents</span></span>

<span data-ttu-id="11ae3-104">O elemento **ReturnQueueEvents** indica que a pessoa que está executando a tarefa está em uma função privilegiada.</span><span class="sxs-lookup"><span data-stu-id="11ae3-104">The **ReturnQueueEvents** element indicates that the person who is running the task is in a privileged role.</span></span> 
  
```XML
<ReturnQueueEvents>true | false</ReturnQueueEvents>
```

 <span data-ttu-id="11ae3-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="11ae3-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="11ae3-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="11ae3-106">Attributes and elements</span></span>

<span data-ttu-id="11ae3-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="11ae3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="11ae3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="11ae3-108">Attributes</span></span>

<span data-ttu-id="11ae3-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11ae3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="11ae3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="11ae3-110">Child elements</span></span>

<span data-ttu-id="11ae3-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="11ae3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="11ae3-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="11ae3-112">Parent elements</span></span>

|<span data-ttu-id="11ae3-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="11ae3-113">**Element**</span></span>|<span data-ttu-id="11ae3-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="11ae3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11ae3-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="11ae3-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="11ae3-116">Contém a solicitação para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) para recuperar o relatório de acompanhamento de mensagens completo da ID especificada.</span><span class="sxs-lookup"><span data-stu-id="11ae3-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="11ae3-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="11ae3-117">Text value</span></span>

<span data-ttu-id="11ae3-118">Um valor de texto que representa um valor booliano é necessário.</span><span class="sxs-lookup"><span data-stu-id="11ae3-118">A text value that represents a Boolean value is required.</span></span> <span data-ttu-id="11ae3-119">Um valor **true** indica que a pessoa que está executando a tarefa está em uma função privilegiada; um valor **false** indica que a pessoa que está executando a tarefa não está em uma função privilegiada.</span><span class="sxs-lookup"><span data-stu-id="11ae3-119">A value of **true** indicates that the person who is running the task is in a privileged role; a value of **false** indicates that the person who is running the task is not in a privileged role.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="11ae3-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="11ae3-120">Remarks</span></span>

<span data-ttu-id="11ae3-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="11ae3-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="11ae3-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="11ae3-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="11ae3-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="11ae3-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="11ae3-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="11ae3-124">Schema Name</span></span>  <br/> |<span data-ttu-id="11ae3-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="11ae3-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="11ae3-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="11ae3-126">Validation File</span></span>  <br/> |<span data-ttu-id="11ae3-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="11ae3-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="11ae3-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="11ae3-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="11ae3-129">False</span><span class="sxs-lookup"><span data-stu-id="11ae3-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="11ae3-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="11ae3-130">See also</span></span>



[<span data-ttu-id="11ae3-131">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="11ae3-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="11ae3-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="11ae3-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

