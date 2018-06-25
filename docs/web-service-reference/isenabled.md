---
title: IsEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsEnabled
api_type:
- schema
ms.assetid: c7e3035e-a4ef-4c11-8cb0-214790a554ff
description: O elemento IsEnabled indica se a regra está habilitada.
ms.openlocfilehash: d0f0a77ec1ec952ac1cd9d9ad686ccfcb8f70c42
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824000"
---
# <a name="isenabled"></a><span data-ttu-id="592dd-103">IsEnabled</span><span class="sxs-lookup"><span data-stu-id="592dd-103">IsEnabled</span></span>

<span data-ttu-id="592dd-104">O elemento **IsEnabled** indica se a regra está habilitada.</span><span class="sxs-lookup"><span data-stu-id="592dd-104">The **IsEnabled** element indicates whether the rule is enabled.</span></span> 
  
```XML
<IsEnabled/>
```

 <span data-ttu-id="592dd-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="592dd-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="592dd-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="592dd-106">Attributes and elements</span></span>

<span data-ttu-id="592dd-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="592dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="592dd-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="592dd-108">Attributes</span></span>

<span data-ttu-id="592dd-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="592dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="592dd-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="592dd-110">Child elements</span></span>

<span data-ttu-id="592dd-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="592dd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="592dd-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="592dd-112">Parent elements</span></span>

|<span data-ttu-id="592dd-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="592dd-113">**Element**</span></span>|<span data-ttu-id="592dd-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="592dd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="592dd-115">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="592dd-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="592dd-116">Representa uma regra de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="592dd-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="592dd-117">Text value</span><span class="sxs-lookup"><span data-stu-id="592dd-117">Text value</span></span>

<span data-ttu-id="592dd-118">Um valor de texto de **true** indica que a regra está habilitada e pode ser executada.</span><span class="sxs-lookup"><span data-stu-id="592dd-118">A text value of **true** indicates that the rule is enabled and can be executed.</span></span> <span data-ttu-id="592dd-119">Um valor **false** indica que a regra não pode ser executada.</span><span class="sxs-lookup"><span data-stu-id="592dd-119">A value of **false** indicates that the rule cannot be executed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="592dd-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="592dd-120">Remarks</span></span>

<span data-ttu-id="592dd-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="592dd-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="592dd-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="592dd-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="592dd-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="592dd-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="592dd-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="592dd-124">Schema Name</span></span>  <br/> |<span data-ttu-id="592dd-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="592dd-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="592dd-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="592dd-126">Validation File</span></span>  <br/> |<span data-ttu-id="592dd-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="592dd-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="592dd-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="592dd-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="592dd-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="592dd-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="592dd-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="592dd-130">See also</span></span>



- [<span data-ttu-id="592dd-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="592dd-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

