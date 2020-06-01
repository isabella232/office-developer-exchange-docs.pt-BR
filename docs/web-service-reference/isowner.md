---
title: IsOwner
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ea0f0afc-32fe-46cb-8530-62a6ce9490f6
description: O elemento IsOwner especifica se o usuário de email especificado é o proprietário.
ms.openlocfilehash: 2dd085aba34052d95efd1e72edca7be4aba71155
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466518"
---
# <a name="isowner"></a><span data-ttu-id="91acb-103">IsOwner</span><span class="sxs-lookup"><span data-stu-id="91acb-103">IsOwner</span></span>

<span data-ttu-id="91acb-104">O elemento **IsOwner** especifica se o usuário de email especificado é o proprietário.</span><span class="sxs-lookup"><span data-stu-id="91acb-104">The **IsOwner** element specifies whether the specified email user is the owner.</span></span> 
  
```XML
<IsOwner>true | false</IsOwner>
```

 <span data-ttu-id="91acb-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="91acb-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="91acb-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="91acb-106">Attributes and elements</span></span>

<span data-ttu-id="91acb-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="91acb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91acb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="91acb-108">Attributes</span></span>

<span data-ttu-id="91acb-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="91acb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="91acb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="91acb-110">Child elements</span></span>

<span data-ttu-id="91acb-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="91acb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="91acb-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="91acb-112">Parent elements</span></span>

|<span data-ttu-id="91acb-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="91acb-113">**Element**</span></span>|<span data-ttu-id="91acb-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="91acb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91acb-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="91acb-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="91acb-116">Especifica informações sobre a licença de gerenciamento de direitos.</span><span class="sxs-lookup"><span data-stu-id="91acb-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="91acb-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="91acb-117">Text value</span></span>

<span data-ttu-id="91acb-118">Um valor de texto **true** para o elemento **IsOwner** indica que o usuário é o proprietário de direitos emitidos em um item.</span><span class="sxs-lookup"><span data-stu-id="91acb-118">A text value of **true** for the **IsOwner** element indicates that the user is the owner of rights issued on an item.</span></span> <span data-ttu-id="91acb-119">Um valor **false** indica que o usuário não é o proprietário dos direitos emitidos em um item.</span><span class="sxs-lookup"><span data-stu-id="91acb-119">A value of **false** indicates that the user is not the owner of rights issued on an item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="91acb-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="91acb-120">Remarks</span></span>

<span data-ttu-id="91acb-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="91acb-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="91acb-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="91acb-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="91acb-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="91acb-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91acb-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="91acb-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="91acb-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="91acb-125">Schema Name</span></span>  <br/> |<span data-ttu-id="91acb-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="91acb-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="91acb-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="91acb-127">Validation File</span></span>  <br/> |<span data-ttu-id="91acb-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="91acb-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="91acb-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="91acb-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="91acb-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="91acb-130">See also</span></span>



- [<span data-ttu-id="91acb-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="91acb-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

