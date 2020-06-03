---
title: ForwardAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bc32e0f4-61e9-4c9f-9a03-90a07eb51c53
description: O elemento ForwardAllowed especifica se o encaminhamento de emails está habilitado.
ms.openlocfilehash: 3c722809bf68239c7d776108cb60d98afbed6e93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461930"
---
# <a name="forwardallowed"></a><span data-ttu-id="5c066-103">ForwardAllowed</span><span class="sxs-lookup"><span data-stu-id="5c066-103">ForwardAllowed</span></span>

<span data-ttu-id="5c066-104">O elemento **ForwardAllowed** especifica se o encaminhamento de emails está habilitado.</span><span class="sxs-lookup"><span data-stu-id="5c066-104">The **ForwardAllowed** element specifies whether forwarding emails is enabled.</span></span> 
  
```XML
<ForwardAllowed>true | false</ForwardAllowed>
```

 <span data-ttu-id="5c066-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="5c066-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c066-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5c066-106">Attributes and elements</span></span>

<span data-ttu-id="5c066-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5c066-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c066-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5c066-108">Attributes</span></span>

<span data-ttu-id="5c066-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5c066-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c066-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5c066-110">Child elements</span></span>

<span data-ttu-id="5c066-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5c066-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5c066-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5c066-112">Parent elements</span></span>

|<span data-ttu-id="5c066-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5c066-113">**Element**</span></span>|<span data-ttu-id="5c066-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5c066-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c066-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="5c066-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="5c066-116">Especifica informações sobre a licença de gerenciamento de direitos.</span><span class="sxs-lookup"><span data-stu-id="5c066-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5c066-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5c066-117">Text value</span></span>

<span data-ttu-id="5c066-118">Um valor de texto **true** para o elemento **ForwardAllowed** indica que o encaminhamento de emails é permitido.</span><span class="sxs-lookup"><span data-stu-id="5c066-118">A text value of **true** for the **ForwardAllowed** element indicates that forwarding emails is allowed.</span></span> <span data-ttu-id="5c066-119">Um valor **false** indica que o encaminhamento não é permitido.</span><span class="sxs-lookup"><span data-stu-id="5c066-119">A value of **false** indicates that forwarding is not allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5c066-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="5c066-120">Remarks</span></span>

<span data-ttu-id="5c066-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5c066-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5c066-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c066-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c066-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5c066-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c066-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="5c066-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5c066-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5c066-125">Schema Name</span></span>  <br/> |<span data-ttu-id="5c066-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="5c066-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="5c066-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5c066-127">Validation File</span></span>  <br/> |<span data-ttu-id="5c066-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5c066-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="5c066-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="5c066-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="5c066-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="5c066-130">See also</span></span>



- [<span data-ttu-id="5c066-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5c066-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

