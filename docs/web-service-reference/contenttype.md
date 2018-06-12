---
title: ContentType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContentType
api_type:
- schema
ms.assetid: f91ff0df-0d8a-43ea-a188-d80f0e885f19
description: Elemento ContentType descreve o tipo de email extensões MIME (Multipurpose Internet) do conteúdo do anexo.
ms.openlocfilehash: 489df47343051623d5b6a98557f2bd434a5dad52
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751513"
---
# <a name="contenttype"></a><span data-ttu-id="26ad7-103">ContentType</span><span class="sxs-lookup"><span data-stu-id="26ad7-103">ContentType</span></span>

<span data-ttu-id="26ad7-104">Elemento **ContentType** descreve o tipo de email extensões MIME (Multipurpose Internet) do conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="26ad7-104">The **ContentType** element describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span> 
  
```xml
<ContentType/>
```

 <span data-ttu-id="26ad7-105">**String**</span><span class="sxs-lookup"><span data-stu-id="26ad7-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26ad7-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="26ad7-106">Attributes and elements</span></span>

<span data-ttu-id="26ad7-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="26ad7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26ad7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="26ad7-108">Attributes</span></span>

<span data-ttu-id="26ad7-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="26ad7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26ad7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="26ad7-110">Child elements</span></span>

<span data-ttu-id="26ad7-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="26ad7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="26ad7-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="26ad7-112">Parent elements</span></span>

|<span data-ttu-id="26ad7-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="26ad7-113">**Element**</span></span>|<span data-ttu-id="26ad7-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="26ad7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26ad7-115">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="26ad7-115">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="26ad7-116">Representa um item do Exchange que está anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="26ad7-116">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="26ad7-117">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="26ad7-117">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="26ad7-118">Representa um arquivo anexado a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="26ad7-118">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="26ad7-119">Text value</span><span class="sxs-lookup"><span data-stu-id="26ad7-119">Text value</span></span>

<span data-ttu-id="26ad7-120">O valor de texto é um valor string que representa o tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="26ad7-120">The text value is a string value that represents the content type of the attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="26ad7-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="26ad7-121">Remarks</span></span>

<span data-ttu-id="26ad7-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="26ad7-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26ad7-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="26ad7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26ad7-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="26ad7-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="26ad7-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="26ad7-125">Schema name</span></span>  <br/> |<span data-ttu-id="26ad7-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="26ad7-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="26ad7-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="26ad7-127">Validation file</span></span>  <br/> |<span data-ttu-id="26ad7-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="26ad7-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="26ad7-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="26ad7-129">Can be empty</span></span>  <br/> |<span data-ttu-id="26ad7-130">False</span><span class="sxs-lookup"><span data-stu-id="26ad7-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="26ad7-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="26ad7-131">See also</span></span>



- [<span data-ttu-id="26ad7-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="26ad7-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

