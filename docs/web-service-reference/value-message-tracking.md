---
title: Valor (controle de mensagens)
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
description: O elemento value representa o valor da propriedade de um relatório de controle de mensagens.
ms.openlocfilehash: 4f6b5cb9d82a35bbe010b36e409cdc9f3a70173d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465005"
---
# <a name="value-message-tracking"></a><span data-ttu-id="c64bc-103">Valor (controle de mensagens)</span><span class="sxs-lookup"><span data-stu-id="c64bc-103">Value (Message Tracking)</span></span>

<span data-ttu-id="c64bc-104">O elemento **Value** representa o valor da propriedade de um relatório de controle de mensagens.</span><span class="sxs-lookup"><span data-stu-id="c64bc-104">The **Value** element represents the property value for a message tracking report.</span></span> 
  
```xml
<Value/>
```

<span data-ttu-id="c64bc-105">**String**</span><span class="sxs-lookup"><span data-stu-id="c64bc-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c64bc-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c64bc-106">Attributes and elements</span></span>

<span data-ttu-id="c64bc-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c64bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c64bc-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c64bc-108">Attributes</span></span>

<span data-ttu-id="c64bc-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c64bc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c64bc-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c64bc-110">Child elements</span></span>

<span data-ttu-id="c64bc-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c64bc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c64bc-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c64bc-112">Parent elements</span></span>

|<span data-ttu-id="c64bc-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c64bc-113">**Element**</span></span>|<span data-ttu-id="c64bc-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c64bc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c64bc-115">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="c64bc-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="c64bc-116">Representa um par de nome e valor de cadeias de caracteres que é usado para criar propriedades para relatórios de controle de mensagens.</span><span class="sxs-lookup"><span data-stu-id="c64bc-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c64bc-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c64bc-117">Text value</span></span>

<span data-ttu-id="c64bc-118">O valor de texto é opcional.</span><span class="sxs-lookup"><span data-stu-id="c64bc-118">The text value is optional.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c64bc-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="c64bc-119">Remarks</span></span>

<span data-ttu-id="c64bc-120">Esse elemento pode ocorrer no máximo uma vez no elemento [TrackingPropertyType](trackingpropertytype.md) .</span><span class="sxs-lookup"><span data-stu-id="c64bc-120">This element can occur at most one time in the [TrackingPropertyType](trackingpropertytype.md) element.</span></span> 
  
<span data-ttu-id="c64bc-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c64bc-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c64bc-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c64bc-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c64bc-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="c64bc-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c64bc-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c64bc-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c64bc-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c64bc-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="c64bc-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c64bc-126">Validation File</span></span>  <br/> |<span data-ttu-id="c64bc-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c64bc-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c64bc-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c64bc-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="c64bc-129">False</span><span class="sxs-lookup"><span data-stu-id="c64bc-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c64bc-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="c64bc-130">See also</span></span>

- [<span data-ttu-id="c64bc-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c64bc-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

