---
title: ContentLocation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContentLocation
api_type:
- schema
ms.assetid: d91cf587-24e3-4c13-8784-5ca29787cca7
description: O elemento ContentLocation contém o identificador de URI (Uniform Resource) que corresponde ao local do conteúdo de um anexo.
ms.openlocfilehash: 060dab2da653637420d5900bad3b95823c2e6ea3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751508"
---
# <a name="contentlocation"></a><span data-ttu-id="14c07-103">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="14c07-103">ContentLocation</span></span>

<span data-ttu-id="14c07-104">O elemento **ContentLocation** contém o identificador de URI (Uniform Resource) que corresponde ao local do conteúdo de um anexo.</span><span class="sxs-lookup"><span data-stu-id="14c07-104">The **ContentLocation** element contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of an attachment.</span></span> 
  
```xml
<ContentLocation/>
```

 <span data-ttu-id="14c07-105">**String**</span><span class="sxs-lookup"><span data-stu-id="14c07-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="14c07-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="14c07-106">Attributes and elements</span></span>

<span data-ttu-id="14c07-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="14c07-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="14c07-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="14c07-108">Attributes</span></span>

<span data-ttu-id="14c07-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="14c07-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="14c07-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="14c07-110">Child elements</span></span>

<span data-ttu-id="14c07-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="14c07-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="14c07-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="14c07-112">Parent elements</span></span>

|<span data-ttu-id="14c07-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="14c07-113">**Element**</span></span>|<span data-ttu-id="14c07-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="14c07-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14c07-115">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="14c07-115">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="14c07-116">Representa um item do Exchange que está anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="14c07-116">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="14c07-117">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="14c07-117">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="14c07-118">Representa um arquivo anexado a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="14c07-118">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="14c07-119">Text value</span><span class="sxs-lookup"><span data-stu-id="14c07-119">Text value</span></span>

<span data-ttu-id="14c07-120">O valor de texto é um valor string que representa um URI.</span><span class="sxs-lookup"><span data-stu-id="14c07-120">The text value is a string value that represents a URI.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="14c07-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="14c07-121">Remarks</span></span>

<span data-ttu-id="14c07-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="14c07-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="14c07-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="14c07-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="14c07-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="14c07-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="14c07-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="14c07-125">Schema name</span></span>  <br/> |<span data-ttu-id="14c07-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="14c07-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="14c07-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="14c07-127">Validation file</span></span>  <br/> |<span data-ttu-id="14c07-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="14c07-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="14c07-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="14c07-129">Can be empty</span></span>  <br/> |<span data-ttu-id="14c07-130">False</span><span class="sxs-lookup"><span data-stu-id="14c07-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="14c07-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="14c07-131">See also</span></span>



- [<span data-ttu-id="14c07-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="14c07-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

