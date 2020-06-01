---
title: EditAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e63c4f7e-77c0-4826-b4e2-43b795d03914
description: O elemento EditAllowed especifica se o gerenciamento de direitos de informação pode ser editado.
ms.openlocfilehash: 979fbaa9fcfbd1015468a8ae00628959bad0bf56
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463479"
---
# <a name="editallowed"></a><span data-ttu-id="2485c-103">EditAllowed</span><span class="sxs-lookup"><span data-stu-id="2485c-103">EditAllowed</span></span>

<span data-ttu-id="2485c-104">O elemento **EditAllowed** especifica se o gerenciamento de direitos de informação pode ser editado.</span><span class="sxs-lookup"><span data-stu-id="2485c-104">The **EditAllowed** element specifies whether Information Rights Management can be edited.</span></span> 
  
```XML
<EditAllowed> true | false </EditAllowed>
```

 <span data-ttu-id="2485c-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="2485c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2485c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2485c-106">Attributes and elements</span></span>

<span data-ttu-id="2485c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2485c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2485c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2485c-108">Attributes</span></span>

<span data-ttu-id="2485c-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2485c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2485c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2485c-110">Child elements</span></span>

<span data-ttu-id="2485c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2485c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2485c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2485c-112">Parent elements</span></span>

|<span data-ttu-id="2485c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2485c-113">**Element**</span></span>|<span data-ttu-id="2485c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2485c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2485c-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="2485c-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="2485c-116">Especifica informações sobre a licença de gerenciamento de direitos.</span><span class="sxs-lookup"><span data-stu-id="2485c-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2485c-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="2485c-117">Text value</span></span>

<span data-ttu-id="2485c-118">Um valor de texto **true** para o elemento **EditAllowed** indica que o gerenciamento de direitos de informação (IRM) pode ser editado.</span><span class="sxs-lookup"><span data-stu-id="2485c-118">A text value of **true** for the **EditAllowed** element indicates that Information Rights Management (IRM) can be edited.</span></span> <span data-ttu-id="2485c-119">Um valor **false** indica que o IRM não pode ser editado.</span><span class="sxs-lookup"><span data-stu-id="2485c-119">A value of **false** indicates that IRM cannot be edited.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2485c-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="2485c-120">Remarks</span></span>

<span data-ttu-id="2485c-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2485c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2485c-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2485c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2485c-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2485c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2485c-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="2485c-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2485c-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2485c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2485c-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="2485c-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="2485c-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2485c-127">Validation File</span></span>  <br/> |<span data-ttu-id="2485c-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2485c-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2485c-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="2485c-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2485c-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="2485c-130">See also</span></span>



- [<span data-ttu-id="2485c-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2485c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

