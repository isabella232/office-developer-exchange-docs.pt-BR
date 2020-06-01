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
ms.openlocfilehash: 7ba7be69868cb439177702f74ff4a2f12875b7ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468352"
---
# <a name="umenabled"></a><span data-ttu-id="94f69-103">UmEnabled</span><span class="sxs-lookup"><span data-stu-id="94f69-103">UmEnabled</span></span>

<span data-ttu-id="94f69-104">O elemento **UmEnabled** indica se a Unificação de mensagens está habilitada para uma conta.</span><span class="sxs-lookup"><span data-stu-id="94f69-104">The **UmEnabled** element indicates whether Unified Messaging is enabled for an account.</span></span> 
  
```XML
<UmEnabled>true | false</UmEnabled>
```

 <span data-ttu-id="94f69-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="94f69-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94f69-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="94f69-106">Attributes and elements</span></span>

<span data-ttu-id="94f69-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="94f69-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94f69-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="94f69-108">Attributes</span></span>

<span data-ttu-id="94f69-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94f69-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="94f69-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="94f69-110">Child elements</span></span>

<span data-ttu-id="94f69-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="94f69-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="94f69-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="94f69-112">Parent elements</span></span>

|<span data-ttu-id="94f69-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="94f69-113">**Element**</span></span>|<span data-ttu-id="94f69-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="94f69-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94f69-115">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="94f69-115">UnifiedMessagingConfiguration</span></span>](unifiedmessagingconfiguration.md) <br/> |<span data-ttu-id="94f69-116">Contém informações de configuração de serviço para o serviço de Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="94f69-116">Contains service configuration information for the Unified Messaging service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="94f69-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="94f69-117">Text value</span></span>

<span data-ttu-id="94f69-118">O valor de texto do elemento **UmEnabled** será **true** se a Unificação de mensagens estiver habilitada para a conta; caso contrário, o valor será **false**.</span><span class="sxs-lookup"><span data-stu-id="94f69-118">The text value of the **UmEnabled** element is **true** if Unified Messaging is enabled for the account; otherwise, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="94f69-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="94f69-119">Remarks</span></span>

<span data-ttu-id="94f69-120">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94f69-120">This element is required.</span></span>
  
<span data-ttu-id="94f69-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="94f69-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94f69-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="94f69-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94f69-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="94f69-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="94f69-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="94f69-124">Schema Name</span></span>  <br/> |<span data-ttu-id="94f69-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="94f69-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="94f69-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="94f69-126">Validation File</span></span>  <br/> |<span data-ttu-id="94f69-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="94f69-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="94f69-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="94f69-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="94f69-129">False</span><span class="sxs-lookup"><span data-stu-id="94f69-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="94f69-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="94f69-130">See also</span></span>



- [<span data-ttu-id="94f69-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="94f69-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

