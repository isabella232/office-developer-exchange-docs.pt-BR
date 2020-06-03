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
description: O elemento ContentId representa um identificador para o conteúdo de um anexo. ContentId pode ser definido como qualquer valor de cadeia de caracteres. Os aplicativos podem usar ContentId para implementar seus próprios mecanismos de identificação.
ms.openlocfilehash: ca89c8790e839326412003f26b738ad1ee956211
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529263"
---
# <a name="contentid"></a><span data-ttu-id="17e25-105">ContentId</span><span class="sxs-lookup"><span data-stu-id="17e25-105">ContentId</span></span>

<span data-ttu-id="17e25-106">O elemento **ContentId** representa um identificador para o conteúdo de um anexo.</span><span class="sxs-lookup"><span data-stu-id="17e25-106">The **ContentId** element represents an identifier for the contents of an attachment.</span></span> <span data-ttu-id="17e25-107">**ContentId** pode ser definido como qualquer valor de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="17e25-107">**ContentId** can be set to any string value.</span></span> <span data-ttu-id="17e25-108">Os aplicativos podem usar **ContentId** para implementar seus próprios mecanismos de identificação.</span><span class="sxs-lookup"><span data-stu-id="17e25-108">Applications can use **ContentId** to implement their own identification mechanisms.</span></span> 
  
```xml
<ContentId/>
```

 <span data-ttu-id="17e25-109">**String**</span><span class="sxs-lookup"><span data-stu-id="17e25-109">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="17e25-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="17e25-110">Attributes and elements</span></span>

<span data-ttu-id="17e25-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="17e25-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="17e25-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="17e25-112">Attributes</span></span>

<span data-ttu-id="17e25-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="17e25-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="17e25-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="17e25-114">Child elements</span></span>

<span data-ttu-id="17e25-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="17e25-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="17e25-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="17e25-116">Parent elements</span></span>

|<span data-ttu-id="17e25-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="17e25-117">**Element**</span></span>|<span data-ttu-id="17e25-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="17e25-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17e25-119">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="17e25-119">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="17e25-120">Representa um item do Exchange anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="17e25-120">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="17e25-121">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="17e25-121">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="17e25-122">Representa um arquivo anexado a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="17e25-122">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="17e25-123">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="17e25-123">Text value</span></span>

<span data-ttu-id="17e25-124">O valor da cadeia de caracteres representa o identificador para o conteúdo de um anexo.</span><span class="sxs-lookup"><span data-stu-id="17e25-124">The string value represents the identifier to the contents of an attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="17e25-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="17e25-125">Remarks</span></span>

<span data-ttu-id="17e25-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="17e25-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="17e25-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="17e25-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="17e25-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="17e25-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="17e25-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="17e25-129">Schema name</span></span>  <br/> |<span data-ttu-id="17e25-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="17e25-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="17e25-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="17e25-131">Validation file</span></span>  <br/> |<span data-ttu-id="17e25-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="17e25-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="17e25-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="17e25-133">Can be empty</span></span>  <br/> |<span data-ttu-id="17e25-134">False</span><span class="sxs-lookup"><span data-stu-id="17e25-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="17e25-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="17e25-135">See also</span></span>



- [<span data-ttu-id="17e25-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="17e25-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

