---
title: EditAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e63c4f7e-77c0-4826-b4e2-43b795d03914
description: O elemento EditAllowed Especifica se o gerenciamento de direitos de informação pode ser editado.
ms.openlocfilehash: 48c7d751c018bf5702b05b41eeaa7ad350189e3a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751960"
---
# <a name="editallowed"></a><span data-ttu-id="b82d8-103">EditAllowed</span><span class="sxs-lookup"><span data-stu-id="b82d8-103">EditAllowed</span></span>

<span data-ttu-id="b82d8-104">O elemento **EditAllowed** Especifica se o gerenciamento de direitos de informação pode ser editado.</span><span class="sxs-lookup"><span data-stu-id="b82d8-104">The **EditAllowed** element specifies whether Information Rights Management can be edited.</span></span> 
  
```XML
<EditAllowed> true | false </EditAllowed>
```

 <span data-ttu-id="b82d8-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="b82d8-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b82d8-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b82d8-106">Attributes and elements</span></span>

<span data-ttu-id="b82d8-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b82d8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b82d8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b82d8-108">Attributes</span></span>

<span data-ttu-id="b82d8-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b82d8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b82d8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b82d8-110">Child elements</span></span>

<span data-ttu-id="b82d8-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b82d8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b82d8-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b82d8-112">Parent elements</span></span>

|<span data-ttu-id="b82d8-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b82d8-113">**Element**</span></span>|<span data-ttu-id="b82d8-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b82d8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b82d8-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="b82d8-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="b82d8-116">Especifica informações sobre a licença de gerenciamento de direitos.</span><span class="sxs-lookup"><span data-stu-id="b82d8-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b82d8-117">Text value</span><span class="sxs-lookup"><span data-stu-id="b82d8-117">Text value</span></span>

<span data-ttu-id="b82d8-118">Um valor de texto de **true** para o elemento **EditAllowed** indica que o gerenciamento de direitos de informação (IRM) pode ser editado.</span><span class="sxs-lookup"><span data-stu-id="b82d8-118">A text value of **true** for the **EditAllowed** element indicates that Information Rights Management (IRM) can be edited.</span></span> <span data-ttu-id="b82d8-119">Um valor **false** indica que o IRM não pode ser editado.</span><span class="sxs-lookup"><span data-stu-id="b82d8-119">A value of **false** indicates that IRM cannot be edited.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b82d8-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="b82d8-120">Remarks</span></span>

<span data-ttu-id="b82d8-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b82d8-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b82d8-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b82d8-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b82d8-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b82d8-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b82d8-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="b82d8-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b82d8-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b82d8-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b82d8-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="b82d8-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="b82d8-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b82d8-127">Validation File</span></span>  <br/> |<span data-ttu-id="b82d8-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b82d8-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b82d8-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b82d8-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b82d8-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="b82d8-130">See also</span></span>



- [<span data-ttu-id="b82d8-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b82d8-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

