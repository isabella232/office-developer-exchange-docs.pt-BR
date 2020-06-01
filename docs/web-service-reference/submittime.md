---
title: Enviartime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubmitTime
api_type:
- schema
ms.assetid: 97e4b71e-f45c-4bdb-80f9-805934916c0f
description: O elemento Submittime representa a hora em que a mensagem foi enviada para o servidor.
ms.openlocfilehash: e4409d962988ee308e0c0b461f9448ef68067fe8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467050"
---
# <a name="submittime"></a><span data-ttu-id="95bae-103">Enviartime</span><span class="sxs-lookup"><span data-stu-id="95bae-103">SubmitTime</span></span>

<span data-ttu-id="95bae-104">O elemento **submittime** representa a hora em que a mensagem foi enviada para o servidor.</span><span class="sxs-lookup"><span data-stu-id="95bae-104">The **SubmitTime** element represents the time at which the message was sent to the server.</span></span> 
  
```XML
<SubmitTime/>
```

 <span data-ttu-id="95bae-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="95bae-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="95bae-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="95bae-106">Attributes and elements</span></span>

<span data-ttu-id="95bae-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="95bae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="95bae-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="95bae-108">Attributes</span></span>

<span data-ttu-id="95bae-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="95bae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="95bae-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="95bae-110">Child elements</span></span>

<span data-ttu-id="95bae-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="95bae-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="95bae-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="95bae-112">Parent elements</span></span>

|<span data-ttu-id="95bae-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="95bae-113">**Element**</span></span>|<span data-ttu-id="95bae-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="95bae-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95bae-115">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="95bae-115">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="95bae-116">Contém uma única mensagem que é retornada em uma [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="95bae-116">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="95bae-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="95bae-117">Text value</span></span>

<span data-ttu-id="95bae-118">Um valor de texto que representa uma data/hora será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="95bae-118">A text value that represents a date/time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="95bae-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="95bae-119">Remarks</span></span>

<span data-ttu-id="95bae-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="95bae-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="95bae-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="95bae-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="95bae-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="95bae-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="95bae-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="95bae-123">Schema Name</span></span>  <br/> |<span data-ttu-id="95bae-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="95bae-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="95bae-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="95bae-125">Validation File</span></span>  <br/> |<span data-ttu-id="95bae-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="95bae-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="95bae-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="95bae-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="95bae-128">False</span><span class="sxs-lookup"><span data-stu-id="95bae-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="95bae-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="95bae-129">See also</span></span>



[<span data-ttu-id="95bae-130">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="95bae-130">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="95bae-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="95bae-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

