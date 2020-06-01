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
description: O elemento Value identifica um único destinatário ou departamento de remetente.
ms.openlocfilehash: 908ea451800abc343fb6e4d4a4ed98d57223bd23
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465237"
---
# <a name="value-protectionrulevaluetype"></a><span data-ttu-id="13e69-103">Valor (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="13e69-103">Value (ProtectionRuleValueType)</span></span>

<span data-ttu-id="13e69-104">O elemento **Value** identifica um único destinatário ou departamento de remetente.</span><span class="sxs-lookup"><span data-stu-id="13e69-104">The **Value** element identifies a single recipient or sender department.</span></span> 
  
```XML
<Value/>
```

<span data-ttu-id="13e69-105">**ProtectionRuleValueType**</span><span class="sxs-lookup"><span data-stu-id="13e69-105">**ProtectionRuleValueType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="13e69-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="13e69-106">Attributes and elements</span></span>

<span data-ttu-id="13e69-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="13e69-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="13e69-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="13e69-108">Attributes</span></span>

<span data-ttu-id="13e69-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="13e69-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="13e69-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="13e69-110">Child elements</span></span>

<span data-ttu-id="13e69-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="13e69-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="13e69-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="13e69-112">Parent elements</span></span>

|<span data-ttu-id="13e69-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="13e69-113">**Element**</span></span>|<span data-ttu-id="13e69-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="13e69-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13e69-115">Destinatário</span><span class="sxs-lookup"><span data-stu-id="13e69-115">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="13e69-116">Especifica que qualquer destinatário da mensagem de email corresponda a qualquer um dos destinatários especificados nos elementos de **valor** filho.</span><span class="sxs-lookup"><span data-stu-id="13e69-116">Specifies that any recipient of the email message matches any of the specified recipients in the child **Value** elements.</span></span>  <br/> |
|[<span data-ttu-id="13e69-117">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="13e69-117">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="13e69-118">Especifica que o departamento do remetente corresponde a qualquer um dos departamentos especificados nos elementos de **valor** filho.</span><span class="sxs-lookup"><span data-stu-id="13e69-118">Specifies that the department of the sender matches any of the specified departments in the child **Value** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="13e69-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="13e69-119">Text value</span></span>

<span data-ttu-id="13e69-120">Este elemento deve conter um valor de cadeia de caracteres não vazio.</span><span class="sxs-lookup"><span data-stu-id="13e69-120">This element must contain a nonempty string value.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="13e69-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="13e69-121">Remarks</span></span>

<span data-ttu-id="13e69-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="13e69-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="13e69-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="13e69-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="13e69-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="13e69-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="13e69-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="13e69-125">Schema Name</span></span>  <br/> |<span data-ttu-id="13e69-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="13e69-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="13e69-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="13e69-127">Validation File</span></span>  <br/> |<span data-ttu-id="13e69-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="13e69-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="13e69-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="13e69-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="13e69-130">False</span><span class="sxs-lookup"><span data-stu-id="13e69-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="13e69-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="13e69-131">See also</span></span>

- [<span data-ttu-id="13e69-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="13e69-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

