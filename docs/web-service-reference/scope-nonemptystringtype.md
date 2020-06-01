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
description: O elemento Scope especifica o escopo do relatório de controle de mensagens.
ms.openlocfilehash: f86f6198e84e094e61ee569f6d005549316bbb9b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466938"
---
# <a name="scope-nonemptystringtype"></a><span data-ttu-id="c1f63-103">Escopo (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="c1f63-103">Scope (NonEmptyStringType)</span></span>

<span data-ttu-id="c1f63-104">O elemento **Scope** especifica o escopo do relatório de controle de mensagens.</span><span class="sxs-lookup"><span data-stu-id="c1f63-104">The **Scope** element specifies the scope of the message tracking report.</span></span> 
  
```XML
<Scope>Organization | Forest | Site</Scope>
```

 <span data-ttu-id="c1f63-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="c1f63-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c1f63-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c1f63-106">Attributes and elements</span></span>

<span data-ttu-id="c1f63-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c1f63-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c1f63-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c1f63-108">Attributes</span></span>

<span data-ttu-id="c1f63-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c1f63-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c1f63-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c1f63-110">Child elements</span></span>

<span data-ttu-id="c1f63-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c1f63-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c1f63-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c1f63-112">Parent elements</span></span>

<span data-ttu-id="c1f63-113">[FindMessageTrackingReport](findmessagetrackingreport.md)  |  [GetMessageTrackingReport](getmessagetrackingreport.md)</span><span class="sxs-lookup"><span data-stu-id="c1f63-113">[FindMessageTrackingReport](findmessagetrackingreport.md) | [GetMessageTrackingReport](getmessagetrackingreport.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c1f63-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c1f63-114">Text value</span></span>

<span data-ttu-id="c1f63-115">A tabela a seguir lista os valores possíveis para o elemento **escopo** .</span><span class="sxs-lookup"><span data-stu-id="c1f63-115">The following table lists the possible values for the **Scope** element.</span></span> 
  
|<span data-ttu-id="c1f63-116">**Valor**</span><span class="sxs-lookup"><span data-stu-id="c1f63-116">**Value**</span></span>|<span data-ttu-id="c1f63-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c1f63-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c1f63-118">Organização</span><span class="sxs-lookup"><span data-stu-id="c1f63-118">Organization</span></span>  <br/> |<span data-ttu-id="c1f63-119">Os escopos de acompanhamento de mensagens se englobem em uma organização.</span><span class="sxs-lookup"><span data-stu-id="c1f63-119">The message tracking scopes spans across an organization.</span></span>  <br/> |
|<span data-ttu-id="c1f63-120">Floresta</span><span class="sxs-lookup"><span data-stu-id="c1f63-120">Forest</span></span>  <br/> |<span data-ttu-id="c1f63-121">Os escopos de acompanhamento de mensagens se expandem em uma floresta.</span><span class="sxs-lookup"><span data-stu-id="c1f63-121">The message tracking scopes spans across a forest.</span></span>  <br/> |
|<span data-ttu-id="c1f63-122">Site</span><span class="sxs-lookup"><span data-stu-id="c1f63-122">Site</span></span>  <br/> |<span data-ttu-id="c1f63-123">Os escopos de acompanhamento de mensagens se englobem em um site.</span><span class="sxs-lookup"><span data-stu-id="c1f63-123">The message tracking scopes spans across a site.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c1f63-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="c1f63-124">Remarks</span></span>

<span data-ttu-id="c1f63-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1f63-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c1f63-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c1f63-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c1f63-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="c1f63-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c1f63-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c1f63-128">Schema Name</span></span>  <br/> |<span data-ttu-id="c1f63-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c1f63-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c1f63-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c1f63-130">Validation File</span></span>  <br/> |<span data-ttu-id="c1f63-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c1f63-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c1f63-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c1f63-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="c1f63-133">False</span><span class="sxs-lookup"><span data-stu-id="c1f63-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c1f63-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="c1f63-134">See also</span></span>



- [<span data-ttu-id="c1f63-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c1f63-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

