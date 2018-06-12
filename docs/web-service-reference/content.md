---
title: Conteúdo
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Content
api_type:
- schema
ms.assetid: 24f8c54a-505f-4fc0-b7e7-93ad50b97070
description: O elemento de conteúdo contém o conteúdo codificado na Base64 de um anexo de arquivo.
ms.openlocfilehash: 20afe6286d3efaa5da6cdc88e397e88fddb1d8c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751498"
---
# <a name="content"></a><span data-ttu-id="884b9-103">Conteúdo</span><span class="sxs-lookup"><span data-stu-id="884b9-103">Content</span></span>

<span data-ttu-id="884b9-104">O elemento de **conteúdo** contém o conteúdo codificado na Base64 de um anexo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="884b9-104">The **Content** element contains the Base64-encoded contents of a file attachment.</span></span> 
  
```xml
<Content/>
```

 <span data-ttu-id="884b9-105">**Base64Binary**</span><span class="sxs-lookup"><span data-stu-id="884b9-105">**Base64Binary**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="884b9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="884b9-106">Attributes and elements</span></span>

<span data-ttu-id="884b9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="884b9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="884b9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="884b9-108">Attributes</span></span>

<span data-ttu-id="884b9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="884b9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="884b9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="884b9-110">Child elements</span></span>

<span data-ttu-id="884b9-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="884b9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="884b9-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="884b9-112">Parent elements</span></span>

|<span data-ttu-id="884b9-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="884b9-113">**Element**</span></span>|<span data-ttu-id="884b9-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="884b9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="884b9-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="884b9-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="884b9-116">Representa um arquivo t é thattached a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="884b9-116">Represents a file t is thattached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="884b9-117">Text value</span><span class="sxs-lookup"><span data-stu-id="884b9-117">Text value</span></span>

<span data-ttu-id="884b9-118">O valor de cadeia de caracteres representa os dados binários codificado na Base64 de arquivo do anexo.</span><span class="sxs-lookup"><span data-stu-id="884b9-118">The string value represents the Base64-encoded binary data of the file attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="884b9-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="884b9-119">Remarks</span></span>

<span data-ttu-id="884b9-120">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="884b9-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="884b9-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="884b9-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="884b9-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="884b9-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="884b9-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="884b9-123">Schema name</span></span>  <br/> |<span data-ttu-id="884b9-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="884b9-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="884b9-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="884b9-125">Validation file</span></span>  <br/> |<span data-ttu-id="884b9-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="884b9-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="884b9-127">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="884b9-127">Can be empty</span></span>  <br/> |<span data-ttu-id="884b9-128">False</span><span class="sxs-lookup"><span data-stu-id="884b9-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="884b9-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="884b9-129">See also</span></span>



- [<span data-ttu-id="884b9-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="884b9-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

