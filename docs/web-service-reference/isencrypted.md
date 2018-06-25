---
title: IsEncrypted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsEncrypted
api_type:
- schema
ms.assetid: 68a30e92-c2b1-4af5-bb16-ba38afb80c43
description: O elemento IsEncrypted indica se as mensagens de entrada devem ser S/MIME criptografada em ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: 582a1f197d4ee6b60af91b1a178d79163b50052c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824003"
---
# <a name="isencrypted"></a><span data-ttu-id="704e3-103">IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="704e3-103">IsEncrypted</span></span>

<span data-ttu-id="704e3-104">O elemento **IsEncrypted** indica se as mensagens de entrada devem ser S/MIME criptografada em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="704e3-104">The **IsEncrypted** element indicates whether incoming messages must be S/MIME encrypted in order for the condition or exception to apply.</span></span> 
  
```XML
<IsEncrypted>true | false</IsEncrypted>
```

 <span data-ttu-id="704e3-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="704e3-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="704e3-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="704e3-106">Attributes and elements</span></span>

<span data-ttu-id="704e3-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="704e3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="704e3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="704e3-108">Attributes</span></span>

<span data-ttu-id="704e3-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="704e3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="704e3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="704e3-110">Child elements</span></span>

<span data-ttu-id="704e3-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="704e3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="704e3-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="704e3-112">Parent elements</span></span>

|<span data-ttu-id="704e3-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="704e3-113">**Element**</span></span>|<span data-ttu-id="704e3-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="704e3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="704e3-115">Condições</span><span class="sxs-lookup"><span data-stu-id="704e3-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="704e3-116">Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="704e3-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="704e3-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="704e3-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="704e3-118">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="704e3-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="704e3-119">Text value</span><span class="sxs-lookup"><span data-stu-id="704e3-119">Text value</span></span>

<span data-ttu-id="704e3-120">Um valor de texto de **true** indica que a mensagem deve ser S/MIME criptografada em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="704e3-120">A text value of **true** indicates that the message must be S/MIME encrypted in order for the condition or exception to apply.</span></span> <span data-ttu-id="704e3-121">Um valor **false** indica que a mensagem não precisa estar S/MIME em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="704e3-121">A value of **false** indicates that the message does not have to be S/MIME in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="704e3-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="704e3-122">Remarks</span></span>

<span data-ttu-id="704e3-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="704e3-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="704e3-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="704e3-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="704e3-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="704e3-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="704e3-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="704e3-126">Schema Name</span></span>  <br/> |<span data-ttu-id="704e3-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="704e3-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="704e3-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="704e3-128">Validation File</span></span>  <br/> |<span data-ttu-id="704e3-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="704e3-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="704e3-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="704e3-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="704e3-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="704e3-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="704e3-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="704e3-132">See also</span></span>



- [<span data-ttu-id="704e3-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="704e3-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

