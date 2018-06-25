---
title: ForwardAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bc32e0f4-61e9-4c9f-9a03-90a07eb51c53
description: O elemento ForwardAllowed Especifica se o encaminhamento de emails está habilitado.
ms.openlocfilehash: 4baa170a531cc9021102ff2255afc113f40e2348
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752354"
---
# <a name="forwardallowed"></a><span data-ttu-id="2c64c-103">ForwardAllowed</span><span class="sxs-lookup"><span data-stu-id="2c64c-103">ForwardAllowed</span></span>

<span data-ttu-id="2c64c-104">O elemento **ForwardAllowed** Especifica se o encaminhamento de emails está habilitado.</span><span class="sxs-lookup"><span data-stu-id="2c64c-104">The **ForwardAllowed** element specifies whether forwarding emails is enabled.</span></span> 
  
```XML
<ForwardAllowed>true | false</ForwardAllowed>
```

 <span data-ttu-id="2c64c-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="2c64c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2c64c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2c64c-106">Attributes and elements</span></span>

<span data-ttu-id="2c64c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2c64c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2c64c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2c64c-108">Attributes</span></span>

<span data-ttu-id="2c64c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2c64c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2c64c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2c64c-110">Child elements</span></span>

<span data-ttu-id="2c64c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2c64c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2c64c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2c64c-112">Parent elements</span></span>

|<span data-ttu-id="2c64c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2c64c-113">**Element**</span></span>|<span data-ttu-id="2c64c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2c64c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c64c-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="2c64c-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="2c64c-116">Especifica informações sobre a licença de gerenciamento de direitos.</span><span class="sxs-lookup"><span data-stu-id="2c64c-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2c64c-117">Text value</span><span class="sxs-lookup"><span data-stu-id="2c64c-117">Text value</span></span>

<span data-ttu-id="2c64c-118">Um valor de texto de **true** para o elemento **ForwardAllowed** indica que o encaminhamento de emails é permitido.</span><span class="sxs-lookup"><span data-stu-id="2c64c-118">A text value of **true** for the **ForwardAllowed** element indicates that forwarding emails is allowed.</span></span> <span data-ttu-id="2c64c-119">Um valor **false** indica que o encaminhamento não é permitido.</span><span class="sxs-lookup"><span data-stu-id="2c64c-119">A value of **false** indicates that forwarding is not allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2c64c-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="2c64c-120">Remarks</span></span>

<span data-ttu-id="2c64c-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2c64c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2c64c-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2c64c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2c64c-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2c64c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2c64c-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="2c64c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2c64c-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2c64c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2c64c-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="2c64c-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="2c64c-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2c64c-127">Validation File</span></span>  <br/> |<span data-ttu-id="2c64c-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2c64c-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2c64c-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="2c64c-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2c64c-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="2c64c-130">See also</span></span>



- [<span data-ttu-id="2c64c-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2c64c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

