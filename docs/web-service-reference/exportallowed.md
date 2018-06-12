---
title: ExportAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dcff5ccc-31dc-4941-9f71-d6519133aebb
description: O elemento ExportAllowed Especifica se a exportação está habilitada.
ms.openlocfilehash: 5c07941e0a79394bbdaa1a1f62b20adedfe7a9bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752146"
---
# <a name="exportallowed"></a><span data-ttu-id="41ec6-103">ExportAllowed</span><span class="sxs-lookup"><span data-stu-id="41ec6-103">ExportAllowed</span></span>

<span data-ttu-id="41ec6-104">O elemento **ExportAllowed** Especifica se a exportação está habilitada.</span><span class="sxs-lookup"><span data-stu-id="41ec6-104">The **ExportAllowed** element specifies whether exporting is enabled.</span></span> 
  
```XML
<ExportAllowed>true | false</ExportAllowed>
```

 <span data-ttu-id="41ec6-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="41ec6-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="41ec6-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="41ec6-106">Attributes and elements</span></span>

<span data-ttu-id="41ec6-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="41ec6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41ec6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="41ec6-108">Attributes</span></span>

<span data-ttu-id="41ec6-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="41ec6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="41ec6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="41ec6-110">Child elements</span></span>

<span data-ttu-id="41ec6-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="41ec6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="41ec6-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="41ec6-112">Parent elements</span></span>

|<span data-ttu-id="41ec6-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="41ec6-113">**Element**</span></span>|<span data-ttu-id="41ec6-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41ec6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41ec6-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="41ec6-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="41ec6-116">Especifica informações sobre a licença de gerenciamento de direitos.</span><span class="sxs-lookup"><span data-stu-id="41ec6-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="41ec6-117">Text value</span><span class="sxs-lookup"><span data-stu-id="41ec6-117">Text value</span></span>

<span data-ttu-id="41ec6-118">Um valor de texto de **true** para o elemento **ExportAllowed** indica que a exportação é permitida.</span><span class="sxs-lookup"><span data-stu-id="41ec6-118">A text value of **true** for the **ExportAllowed** element indicates that exporting is allowed.</span></span> <span data-ttu-id="41ec6-119">Um valor **false** indica que não é permitida a exportação.</span><span class="sxs-lookup"><span data-stu-id="41ec6-119">A value of **false** indicates that exporting is not allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="41ec6-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="41ec6-120">Remarks</span></span>

<span data-ttu-id="41ec6-121">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="41ec6-121">This element is optional.</span></span>
  
<span data-ttu-id="41ec6-122">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="41ec6-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="41ec6-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="41ec6-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="41ec6-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="41ec6-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="41ec6-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="41ec6-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="41ec6-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="41ec6-126">Schema Name</span></span>  <br/> |<span data-ttu-id="41ec6-127">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="41ec6-127">Type schema</span></span>  <br/> |
|<span data-ttu-id="41ec6-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="41ec6-128">Validation File</span></span>  <br/> |<span data-ttu-id="41ec6-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="41ec6-129">types.xsd</span></span>  <br/> |
|<span data-ttu-id="41ec6-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="41ec6-130">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="41ec6-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="41ec6-131">See also</span></span>



- [<span data-ttu-id="41ec6-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="41ec6-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

