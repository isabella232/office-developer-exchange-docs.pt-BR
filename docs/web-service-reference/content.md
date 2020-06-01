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
description: O elemento Content contém o conteúdo codificado em Base64 de um anexo de arquivo.
ms.openlocfilehash: 81f6acf69ff702bd0645663cb2e499ee5b45ea78
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458947"
---
# <a name="content"></a><span data-ttu-id="01cc8-103">Conteúdo</span><span class="sxs-lookup"><span data-stu-id="01cc8-103">Content</span></span>

<span data-ttu-id="01cc8-104">O elemento **Content** contém o conteúdo codificado em Base64 de um anexo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="01cc8-104">The **Content** element contains the Base64-encoded contents of a file attachment.</span></span> 
  
```xml
<Content/>
```

 <span data-ttu-id="01cc8-105">**Base64Binary**</span><span class="sxs-lookup"><span data-stu-id="01cc8-105">**Base64Binary**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01cc8-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="01cc8-106">Attributes and elements</span></span>

<span data-ttu-id="01cc8-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="01cc8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01cc8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="01cc8-108">Attributes</span></span>

<span data-ttu-id="01cc8-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="01cc8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01cc8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="01cc8-110">Child elements</span></span>

<span data-ttu-id="01cc8-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="01cc8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="01cc8-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="01cc8-112">Parent elements</span></span>

|<span data-ttu-id="01cc8-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="01cc8-113">**Element**</span></span>|<span data-ttu-id="01cc8-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="01cc8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01cc8-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="01cc8-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="01cc8-116">Representa um arquivo t é thattached a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="01cc8-116">Represents a file t is thattached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="01cc8-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="01cc8-117">Text value</span></span>

<span data-ttu-id="01cc8-118">O valor da cadeia de caracteres representa os dados binários codificados em base64 do anexo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="01cc8-118">The string value represents the Base64-encoded binary data of the file attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="01cc8-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="01cc8-119">Remarks</span></span>

<span data-ttu-id="01cc8-120">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="01cc8-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01cc8-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="01cc8-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01cc8-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="01cc8-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="01cc8-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="01cc8-123">Schema name</span></span>  <br/> |<span data-ttu-id="01cc8-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="01cc8-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="01cc8-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="01cc8-125">Validation file</span></span>  <br/> |<span data-ttu-id="01cc8-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="01cc8-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="01cc8-127">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="01cc8-127">Can be empty</span></span>  <br/> |<span data-ttu-id="01cc8-128">False</span><span class="sxs-lookup"><span data-stu-id="01cc8-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01cc8-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="01cc8-129">See also</span></span>



- [<span data-ttu-id="01cc8-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="01cc8-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

