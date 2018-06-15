---
title: UmEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UmEnabled
api_type:
- schema
ms.assetid: 87382d9b-0c02-49ec-85dc-3f5918df3195
description: O elemento UmEnabled indica se a Unificação de mensagens está habilitada para uma conta.
ms.openlocfilehash: 8324e02136adc6704bc0badb77131e9671ee569f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2018
ms.locfileid: "19837817"
---
# <a name="umenabled"></a><span data-ttu-id="19489-103">UmEnabled</span><span class="sxs-lookup"><span data-stu-id="19489-103">UmEnabled</span></span>

<span data-ttu-id="19489-104">O elemento **UmEnabled** indica se a Unificação de mensagens está habilitada para uma conta.</span><span class="sxs-lookup"><span data-stu-id="19489-104">The **UmEnabled** element indicates whether Unified Messaging is enabled for an account.</span></span> 
  
```XML
<UmEnabled>true | false</UmEnabled>
```

 <span data-ttu-id="19489-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="19489-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19489-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="19489-106">Attributes and elements</span></span>

<span data-ttu-id="19489-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="19489-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19489-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="19489-108">Attributes</span></span>

<span data-ttu-id="19489-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="19489-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19489-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="19489-110">Child elements</span></span>

<span data-ttu-id="19489-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="19489-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="19489-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="19489-112">Parent elements</span></span>

|<span data-ttu-id="19489-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="19489-113">**Element**</span></span>|<span data-ttu-id="19489-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="19489-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19489-115">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="19489-115">UnifiedMessagingConfiguration</span></span>](unifiedmessagingconfiguration.md) <br/> |<span data-ttu-id="19489-116">Contém informações de configuração de serviço para o serviço de Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="19489-116">Contains service configuration information for the Unified Messaging service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="19489-117">Text value</span><span class="sxs-lookup"><span data-stu-id="19489-117">Text value</span></span>

<span data-ttu-id="19489-118">O valor de texto do elemento **UmEnabled** é **true** se a Unificação de mensagens está habilitado para a conta; Caso contrário, o valor é **false**.</span><span class="sxs-lookup"><span data-stu-id="19489-118">The text value of the **UmEnabled** element is **true** if Unified Messaging is enabled for the account; otherwise, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="19489-119">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="19489-119">Remarks</span></span>

<span data-ttu-id="19489-120">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19489-120">This element is required.</span></span>
  
<span data-ttu-id="19489-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="19489-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19489-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="19489-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19489-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="19489-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="19489-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="19489-124">Schema Name</span></span>  <br/> |<span data-ttu-id="19489-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="19489-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="19489-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="19489-126">Validation File</span></span>  <br/> |<span data-ttu-id="19489-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="19489-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="19489-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="19489-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="19489-129">False</span><span class="sxs-lookup"><span data-stu-id="19489-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="19489-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="19489-130">See also</span></span>



- [<span data-ttu-id="19489-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="19489-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

