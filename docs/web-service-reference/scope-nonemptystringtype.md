---
title: Escopo (NonEmptyStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Scope
api_type:
- schema
ms.assetid: 7efb6fd9-1615-469e-96f6-0f7846ad9b44
description: O elemento escopo Especifica o escopo do relatório de controle de mensagens.
ms.openlocfilehash: 534ed23916a60b246c7cb5be4a59d086980a7c37
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825280"
---
# <a name="scope-nonemptystringtype"></a><span data-ttu-id="68661-103">Escopo (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="68661-103">Scope (NonEmptyStringType)</span></span>

<span data-ttu-id="68661-104">O elemento **escopo** Especifica o escopo do relatório de controle de mensagens.</span><span class="sxs-lookup"><span data-stu-id="68661-104">The **Scope** element specifies the scope of the message tracking report.</span></span> 
  
```XML
<Scope>Organization | Forest | Site</Scope>
```

 <span data-ttu-id="68661-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="68661-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="68661-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="68661-106">Attributes and elements</span></span>

<span data-ttu-id="68661-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="68661-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="68661-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="68661-108">Attributes</span></span>

<span data-ttu-id="68661-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="68661-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="68661-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="68661-110">Child elements</span></span>

<span data-ttu-id="68661-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="68661-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="68661-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="68661-112">Parent elements</span></span>

<span data-ttu-id="68661-113">[FindMessageTrackingReport](findmessagetrackingreport.md) | [GetMessageTrackingReport](getmessagetrackingreport.md)</span><span class="sxs-lookup"><span data-stu-id="68661-113">[FindMessageTrackingReport](findmessagetrackingreport.md) | [GetMessageTrackingReport](getmessagetrackingreport.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="68661-114">Text value</span><span class="sxs-lookup"><span data-stu-id="68661-114">Text value</span></span>

<span data-ttu-id="68661-115">A tabela a seguir lista os valores possíveis para o elemento de **escopo** .</span><span class="sxs-lookup"><span data-stu-id="68661-115">The following table lists the possible values for the **Scope** element.</span></span> 
  
|<span data-ttu-id="68661-116">**Valor**</span><span class="sxs-lookup"><span data-stu-id="68661-116">**Value**</span></span>|<span data-ttu-id="68661-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="68661-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="68661-118">Organização</span><span class="sxs-lookup"><span data-stu-id="68661-118">Organization</span></span>  <br/> |<span data-ttu-id="68661-119">Escopos de controle de mensagens abrange em uma organização.</span><span class="sxs-lookup"><span data-stu-id="68661-119">The message tracking scopes spans across an organization.</span></span>  <br/> |
|<span data-ttu-id="68661-120">Floresta</span><span class="sxs-lookup"><span data-stu-id="68661-120">Forest</span></span>  <br/> |<span data-ttu-id="68661-121">Escopos de controle de mensagens abrange em uma floresta.</span><span class="sxs-lookup"><span data-stu-id="68661-121">The message tracking scopes spans across a forest.</span></span>  <br/> |
|<span data-ttu-id="68661-122">Site</span><span class="sxs-lookup"><span data-stu-id="68661-122">Site</span></span>  <br/> |<span data-ttu-id="68661-123">Escopos de controle de mensagens abrange em um site.</span><span class="sxs-lookup"><span data-stu-id="68661-123">The message tracking scopes spans across a site.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="68661-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="68661-124">Remarks</span></span>

<span data-ttu-id="68661-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="68661-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="68661-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="68661-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="68661-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="68661-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="68661-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="68661-128">Schema Name</span></span>  <br/> |<span data-ttu-id="68661-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="68661-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="68661-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="68661-130">Validation File</span></span>  <br/> |<span data-ttu-id="68661-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="68661-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="68661-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="68661-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="68661-133">False</span><span class="sxs-lookup"><span data-stu-id="68661-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="68661-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="68661-134">See also</span></span>



- [<span data-ttu-id="68661-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="68661-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

