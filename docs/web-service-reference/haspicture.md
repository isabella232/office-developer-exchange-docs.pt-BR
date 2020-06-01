---
title: HasPicture
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HasPicture
api_type:
- schema
ms.assetid: 922a43fe-01bd-49f2-9261-e00e4699b8da
description: O elemento HasPicture indica se o item de contato tem um anexo de arquivo que representa a imagem do contato.
ms.openlocfilehash: 0f0758e38807587d47b9469f40b10bd9c6ea5012
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462434"
---
# <a name="haspicture"></a><span data-ttu-id="25f56-103">HasPicture</span><span class="sxs-lookup"><span data-stu-id="25f56-103">HasPicture</span></span>

<span data-ttu-id="25f56-104">O elemento **HasPicture** indica se o item de contato tem um anexo de arquivo que representa a imagem do contato.</span><span class="sxs-lookup"><span data-stu-id="25f56-104">The **HasPicture** element indicates whether the contact item has a file attachment that represents the contact's picture.</span></span> 
  
[<span data-ttu-id="25f56-105">Contato</span><span class="sxs-lookup"><span data-stu-id="25f56-105">Contact</span></span>](contact.md)
  
[<span data-ttu-id="25f56-106">HasPicture</span><span class="sxs-lookup"><span data-stu-id="25f56-106">HasPicture</span></span>](haspicture.md)
  
```xml
<HasPicture>true or false</HasPicture>
```

 <span data-ttu-id="25f56-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="25f56-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="25f56-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="25f56-108">Attributes and elements</span></span>

<span data-ttu-id="25f56-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="25f56-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25f56-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="25f56-110">Attributes</span></span>

<span data-ttu-id="25f56-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25f56-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="25f56-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="25f56-112">Child elements</span></span>

<span data-ttu-id="25f56-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="25f56-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="25f56-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="25f56-114">Parent elements</span></span>

|<span data-ttu-id="25f56-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="25f56-115">**Element**</span></span>|<span data-ttu-id="25f56-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="25f56-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25f56-117">Contato</span><span class="sxs-lookup"><span data-stu-id="25f56-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="25f56-118">Representa um item de contato no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="25f56-118">Represents a contact item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="25f56-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="25f56-119">Text value</span></span>

<span data-ttu-id="25f56-120">O valor de texto do elemento **HasPicture** pode ser **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="25f56-120">The text value of the **HasPicture** element can be either **true** or **false**.</span></span> <span data-ttu-id="25f56-121">O valor padrão é **false**.</span><span class="sxs-lookup"><span data-stu-id="25f56-121">The default value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="25f56-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="25f56-122">Remarks</span></span>

<span data-ttu-id="25f56-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="25f56-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25f56-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="25f56-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25f56-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="25f56-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="25f56-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="25f56-126">Schema Name</span></span>  <br/> |<span data-ttu-id="25f56-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="25f56-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="25f56-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="25f56-128">Validation File</span></span>  <br/> |<span data-ttu-id="25f56-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="25f56-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="25f56-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="25f56-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="25f56-131">False</span><span class="sxs-lookup"><span data-stu-id="25f56-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="25f56-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="25f56-132">See also</span></span>



- [<span data-ttu-id="25f56-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="25f56-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

