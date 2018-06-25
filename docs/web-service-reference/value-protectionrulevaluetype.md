---
title: Valor (ProtectionRuleValueType)
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
ms.assetid: b039bd6e-2198-47cf-9c78-a5e8b9d51c98
description: O elemento de valor identifica um único departamento do destinatário ou o remetente.
ms.openlocfilehash: 6173f94dcfb83eafd62e35f185a5e8c669d50f6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838023"
---
# <a name="value-protectionrulevaluetype"></a><span data-ttu-id="8e9c9-103">Valor (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="8e9c9-103">Value (ProtectionRuleValueType)</span></span>

<span data-ttu-id="8e9c9-104">O elemento de **valor** identifica um único departamento do destinatário ou o remetente.</span><span class="sxs-lookup"><span data-stu-id="8e9c9-104">The **Value** element identifies a single recipient or sender department.</span></span> 
  
```XML
<Value/>
```

<span data-ttu-id="8e9c9-105">**ProtectionRuleValueType**</span><span class="sxs-lookup"><span data-stu-id="8e9c9-105">**ProtectionRuleValueType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8e9c9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8e9c9-106">Attributes and elements</span></span>

<span data-ttu-id="8e9c9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8e9c9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e9c9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8e9c9-108">Attributes</span></span>

<span data-ttu-id="8e9c9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8e9c9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8e9c9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8e9c9-110">Child elements</span></span>

<span data-ttu-id="8e9c9-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8e9c9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8e9c9-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8e9c9-112">Parent elements</span></span>

|<span data-ttu-id="8e9c9-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8e9c9-113">**Element**</span></span>|<span data-ttu-id="8e9c9-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8e9c9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e9c9-115">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="8e9c9-115">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="8e9c9-116">Especifica que qualquer destinatário da mensagem de email corresponde a qualquer um dos destinatários especificados no **valor** elementos filhos.</span><span class="sxs-lookup"><span data-stu-id="8e9c9-116">Specifies that any recipient of the email message matches any of the specified recipients in the child **Value** elements.</span></span>  <br/> |
|[<span data-ttu-id="8e9c9-117">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="8e9c9-117">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="8e9c9-118">Especifica se o departamento do remetente corresponde a um dos departamentos especificados no **valor** elementos filhos.</span><span class="sxs-lookup"><span data-stu-id="8e9c9-118">Specifies that the department of the sender matches any of the specified departments in the child **Value** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8e9c9-119">Text value</span><span class="sxs-lookup"><span data-stu-id="8e9c9-119">Text value</span></span>

<span data-ttu-id="8e9c9-120">Este elemento deve conter um valor de cadeia de caracteres vazia.</span><span class="sxs-lookup"><span data-stu-id="8e9c9-120">This element must contain a nonempty string value.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8e9c9-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="8e9c9-121">Remarks</span></span>

<span data-ttu-id="8e9c9-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e9c9-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8e9c9-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8e9c9-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e9c9-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="8e9c9-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8e9c9-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8e9c9-125">Schema Name</span></span>  <br/> |<span data-ttu-id="8e9c9-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8e9c9-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="8e9c9-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8e9c9-127">Validation File</span></span>  <br/> |<span data-ttu-id="8e9c9-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8e9c9-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8e9c9-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8e9c9-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="8e9c9-130">False</span><span class="sxs-lookup"><span data-stu-id="8e9c9-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8e9c9-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="8e9c9-131">See also</span></span>

- [<span data-ttu-id="8e9c9-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8e9c9-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

