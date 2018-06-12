---
title: Valor (rastreamento de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Value
api_type:
- schema
ms.assetid: cb2f228f-775a-4c7d-82e7-41c7c953c808
description: O elemento de valor representa o valor da propriedade para um relatório de controle de mensagens.
ms.openlocfilehash: 152e4fe61a4cff8013ae02900bd84bf244ae84a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838020"
---
# <a name="value-message-tracking"></a><span data-ttu-id="792ce-103">Valor (rastreamento de mensagens)</span><span class="sxs-lookup"><span data-stu-id="792ce-103">Value (Message Tracking)</span></span>

<span data-ttu-id="792ce-104">O elemento de **valor** representa o valor da propriedade para um relatório de controle de mensagens.</span><span class="sxs-lookup"><span data-stu-id="792ce-104">The **Value** element represents the property value for a message tracking report.</span></span> 
  
```xml
<Value/>
```

<span data-ttu-id="792ce-105">**String**</span><span class="sxs-lookup"><span data-stu-id="792ce-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="792ce-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="792ce-106">Attributes and elements</span></span>

<span data-ttu-id="792ce-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="792ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="792ce-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="792ce-108">Attributes</span></span>

<span data-ttu-id="792ce-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="792ce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="792ce-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="792ce-110">Child elements</span></span>

<span data-ttu-id="792ce-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="792ce-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="792ce-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="792ce-112">Parent elements</span></span>

|<span data-ttu-id="792ce-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="792ce-113">**Element**</span></span>|<span data-ttu-id="792ce-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="792ce-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="792ce-115">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="792ce-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="792ce-116">Representa um par de nome e valor de cadeias de caracteres que é usado para criar propriedades para relatórios de acompanhamento de mensagens.</span><span class="sxs-lookup"><span data-stu-id="792ce-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="792ce-117">Text value</span><span class="sxs-lookup"><span data-stu-id="792ce-117">Text value</span></span>

<span data-ttu-id="792ce-118">O valor de texto é opcional.</span><span class="sxs-lookup"><span data-stu-id="792ce-118">The text value is optional.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="792ce-119">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="792ce-119">Remarks</span></span>

<span data-ttu-id="792ce-120">Esse elemento pode ocorrer no máximo uma vez no elemento [TrackingPropertyType](trackingpropertytype.md) .</span><span class="sxs-lookup"><span data-stu-id="792ce-120">This element can occur at most one time in the [TrackingPropertyType](trackingpropertytype.md) element.</span></span> 
  
<span data-ttu-id="792ce-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="792ce-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="792ce-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="792ce-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="792ce-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="792ce-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="792ce-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="792ce-124">Schema Name</span></span>  <br/> |<span data-ttu-id="792ce-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="792ce-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="792ce-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="792ce-126">Validation File</span></span>  <br/> |<span data-ttu-id="792ce-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="792ce-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="792ce-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="792ce-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="792ce-129">False</span><span class="sxs-lookup"><span data-stu-id="792ce-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="792ce-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="792ce-130">See also</span></span>

- [<span data-ttu-id="792ce-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="792ce-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

