---
title: IsInline
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsInline
api_type:
- schema
ms.assetid: 5e7712c8-372a-4a16-be64-360c5ff3961a
description: O elemento IsInline indica se o anexo é exibido embutida dentro de um item.
ms.openlocfilehash: f2f9093777a3914de067ef63827de6cf354fc12d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824042"
---
# <a name="isinline"></a><span data-ttu-id="f5ee1-103">IsInline</span><span class="sxs-lookup"><span data-stu-id="f5ee1-103">IsInline</span></span>

<span data-ttu-id="f5ee1-104">O elemento **IsInline** indica se o anexo é exibido embutida dentro de um item.</span><span class="sxs-lookup"><span data-stu-id="f5ee1-104">The **IsInline** element represents whether the attachment appears inline within an item.</span></span> 
  
```xml
<IsInline>true or false</IsInline>
```

 <span data-ttu-id="f5ee1-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="f5ee1-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f5ee1-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f5ee1-106">Attributes and elements</span></span>

<span data-ttu-id="f5ee1-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f5ee1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f5ee1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f5ee1-108">Attributes</span></span>

<span data-ttu-id="f5ee1-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f5ee1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f5ee1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f5ee1-110">Child elements</span></span>

<span data-ttu-id="f5ee1-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f5ee1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f5ee1-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f5ee1-112">Parent elements</span></span>

|<span data-ttu-id="f5ee1-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f5ee1-113">**Element**</span></span>|<span data-ttu-id="f5ee1-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f5ee1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5ee1-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="f5ee1-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="f5ee1-116">Representa um arquivo anexado a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5ee1-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f5ee1-117">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="f5ee1-117">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="f5ee1-118">Representa um item do Exchange que está anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5ee1-118">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f5ee1-119">Text value</span><span class="sxs-lookup"><span data-stu-id="f5ee1-119">Text value</span></span>

<span data-ttu-id="f5ee1-120">Esse elemento pode ser **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="f5ee1-120">This element can be either **true** or **false**.</span></span> <span data-ttu-id="f5ee1-121">O valor padrão é **false**.</span><span class="sxs-lookup"><span data-stu-id="f5ee1-121">The default value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f5ee1-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="f5ee1-122">Remarks</span></span>

<span data-ttu-id="f5ee1-123">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f5ee1-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f5ee1-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f5ee1-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f5ee1-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="f5ee1-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f5ee1-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f5ee1-126">Schema Name</span></span>  <br/> |<span data-ttu-id="f5ee1-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f5ee1-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="f5ee1-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f5ee1-128">Validation File</span></span>  <br/> |<span data-ttu-id="f5ee1-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f5ee1-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f5ee1-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f5ee1-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="f5ee1-131">False</span><span class="sxs-lookup"><span data-stu-id="f5ee1-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f5ee1-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="f5ee1-132">See also</span></span>



- [<span data-ttu-id="f5ee1-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f5ee1-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

