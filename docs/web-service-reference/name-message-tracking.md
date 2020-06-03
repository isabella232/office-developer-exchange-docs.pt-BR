---
title: Nome (controle de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: a1669f6d-53f3-4849-9b30-56909aaeac82
description: O elemento name representa o nome da propriedade de um relatório de controle de mensagens.
ms.openlocfilehash: 86f049c0a90dbeb55418a5eee58079adf17e5ded
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466896"
---
# <a name="name-message-tracking"></a><span data-ttu-id="fc0f7-103">Nome (controle de mensagens)</span><span class="sxs-lookup"><span data-stu-id="fc0f7-103">Name (Message Tracking)</span></span>

<span data-ttu-id="fc0f7-104">O elemento **Name** representa o nome da propriedade de um relatório de controle de mensagens.</span><span class="sxs-lookup"><span data-stu-id="fc0f7-104">The **Name** element represents the property name for a message tracking report.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="fc0f7-105">**String**</span><span class="sxs-lookup"><span data-stu-id="fc0f7-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="fc0f7-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fc0f7-106">Attributes and elements</span></span>

<span data-ttu-id="fc0f7-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fc0f7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc0f7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fc0f7-108">Attributes</span></span>

<span data-ttu-id="fc0f7-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc0f7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc0f7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fc0f7-110">Child elements</span></span>

<span data-ttu-id="fc0f7-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fc0f7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fc0f7-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fc0f7-112">Parent elements</span></span>

|<span data-ttu-id="fc0f7-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fc0f7-113">**Element**</span></span>|<span data-ttu-id="fc0f7-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fc0f7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc0f7-115">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="fc0f7-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="fc0f7-116">Representa um par de nome e valor de cadeias de caracteres que é usado para criar propriedades para relatórios de controle de mensagens.</span><span class="sxs-lookup"><span data-stu-id="fc0f7-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fc0f7-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="fc0f7-117">Text value</span></span>

<span data-ttu-id="fc0f7-118">Um valor de texto será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="fc0f7-118">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fc0f7-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="fc0f7-119">Remarks</span></span>

<span data-ttu-id="fc0f7-120">Esse elemento pode ocorrer no máximo uma vez no elemento [TrackingPropertyType](trackingpropertytype.md) .</span><span class="sxs-lookup"><span data-stu-id="fc0f7-120">This element can occur at most one time in the [TrackingPropertyType](trackingpropertytype.md) element.</span></span> 
  
<span data-ttu-id="fc0f7-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="fc0f7-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc0f7-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="fc0f7-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc0f7-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="fc0f7-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fc0f7-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fc0f7-124">Schema Name</span></span>  <br/> |<span data-ttu-id="fc0f7-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="fc0f7-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="fc0f7-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fc0f7-126">Validation File</span></span>  <br/> |<span data-ttu-id="fc0f7-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fc0f7-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fc0f7-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fc0f7-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="fc0f7-129">False</span><span class="sxs-lookup"><span data-stu-id="fc0f7-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc0f7-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="fc0f7-130">See also</span></span>

- [<span data-ttu-id="fc0f7-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fc0f7-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

