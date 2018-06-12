---
title: ContentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContentId
api_type:
- schema
ms.assetid: bc59100d-6079-414b-a6e0-7c15feaa3184
description: O elemento ContentId representa um identificador para o conteúdo de um anexo. ContentId pode ser definido como qualquer valor de cadeia de caracteres. Aplicativos podem usar ContentId implementar seus próprios mecanismos de identificação.
ms.openlocfilehash: dc46ae4b33d435f5d47eb7deb39e92fd0170194b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751505"
---
# <a name="contentid"></a><span data-ttu-id="c0a8c-105">ContentId</span><span class="sxs-lookup"><span data-stu-id="c0a8c-105">ContentId</span></span>

<span data-ttu-id="c0a8c-106">O elemento **ContentId** representa um identificador para o conteúdo de um anexo.</span><span class="sxs-lookup"><span data-stu-id="c0a8c-106">The **ContentId** element represents an identifier for the contents of an attachment.</span></span> <span data-ttu-id="c0a8c-107">**ContentId** pode ser definido como qualquer valor de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="c0a8c-107">**ContentId** can be set to any string value.</span></span> <span data-ttu-id="c0a8c-108">Aplicativos podem usar **ContentId** implementar seus próprios mecanismos de identificação.</span><span class="sxs-lookup"><span data-stu-id="c0a8c-108">Applications can use **ContentId** to implement their own identification mechanisms.</span></span> 
  
```xml
<ContentId/>
```

 <span data-ttu-id="c0a8c-109">**String**</span><span class="sxs-lookup"><span data-stu-id="c0a8c-109">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c0a8c-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c0a8c-110">Attributes and elements</span></span>

<span data-ttu-id="c0a8c-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c0a8c-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0a8c-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="c0a8c-112">Attributes</span></span>

<span data-ttu-id="c0a8c-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c0a8c-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c0a8c-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c0a8c-114">Child elements</span></span>

<span data-ttu-id="c0a8c-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c0a8c-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c0a8c-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c0a8c-116">Parent elements</span></span>

|<span data-ttu-id="c0a8c-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c0a8c-117">**Element**</span></span>|<span data-ttu-id="c0a8c-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c0a8c-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0a8c-119">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="c0a8c-119">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="c0a8c-120">Representa um item do Exchange que está anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c0a8c-120">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="c0a8c-121">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="c0a8c-121">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="c0a8c-122">Representa um arquivo anexado a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c0a8c-122">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c0a8c-123">Text value</span><span class="sxs-lookup"><span data-stu-id="c0a8c-123">Text value</span></span>

<span data-ttu-id="c0a8c-124">O valor de cadeia de caracteres representa o identificador para o conteúdo de um anexo.</span><span class="sxs-lookup"><span data-stu-id="c0a8c-124">The string value represents the identifier to the contents of an attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c0a8c-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="c0a8c-125">Remarks</span></span>

<span data-ttu-id="c0a8c-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="c0a8c-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c0a8c-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c0a8c-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0a8c-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="c0a8c-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c0a8c-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c0a8c-129">Schema name</span></span>  <br/> |<span data-ttu-id="c0a8c-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c0a8c-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="c0a8c-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c0a8c-131">Validation file</span></span>  <br/> |<span data-ttu-id="c0a8c-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c0a8c-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c0a8c-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="c0a8c-133">Can be empty</span></span>  <br/> |<span data-ttu-id="c0a8c-134">False</span><span class="sxs-lookup"><span data-stu-id="c0a8c-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c0a8c-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="c0a8c-135">See also</span></span>



- [<span data-ttu-id="c0a8c-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c0a8c-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

