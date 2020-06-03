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
description: O elemento IsInline indica se o anexo aparece embutido em um item.
ms.openlocfilehash: 2b3b6392fe8867ae9782dcb7211c17f4f4d9becd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464207"
---
# <a name="isinline"></a><span data-ttu-id="f5053-103">IsInline</span><span class="sxs-lookup"><span data-stu-id="f5053-103">IsInline</span></span>

<span data-ttu-id="f5053-104">O elemento **IsInline** indica se o anexo aparece embutido em um item.</span><span class="sxs-lookup"><span data-stu-id="f5053-104">The **IsInline** element represents whether the attachment appears inline within an item.</span></span> 
  
```xml
<IsInline>true or false</IsInline>
```

 <span data-ttu-id="f5053-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="f5053-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f5053-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f5053-106">Attributes and elements</span></span>

<span data-ttu-id="f5053-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f5053-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f5053-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f5053-108">Attributes</span></span>

<span data-ttu-id="f5053-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f5053-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f5053-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f5053-110">Child elements</span></span>

<span data-ttu-id="f5053-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f5053-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f5053-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f5053-112">Parent elements</span></span>

|<span data-ttu-id="f5053-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f5053-113">**Element**</span></span>|<span data-ttu-id="f5053-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f5053-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5053-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="f5053-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="f5053-116">Representa um arquivo anexado a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5053-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f5053-117">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="f5053-117">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="f5053-118">Representa um item do Exchange anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5053-118">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f5053-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="f5053-119">Text value</span></span>

<span data-ttu-id="f5053-120">Esse elemento pode ser **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="f5053-120">This element can be either **true** or **false**.</span></span> <span data-ttu-id="f5053-121">O valor padrão é **false**.</span><span class="sxs-lookup"><span data-stu-id="f5053-121">The default value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f5053-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="f5053-122">Remarks</span></span>

<span data-ttu-id="f5053-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f5053-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f5053-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f5053-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f5053-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="f5053-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f5053-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f5053-126">Schema Name</span></span>  <br/> |<span data-ttu-id="f5053-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f5053-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="f5053-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f5053-128">Validation File</span></span>  <br/> |<span data-ttu-id="f5053-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f5053-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f5053-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f5053-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="f5053-131">False</span><span class="sxs-lookup"><span data-stu-id="f5053-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f5053-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="f5053-132">See also</span></span>



- [<span data-ttu-id="f5053-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f5053-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

