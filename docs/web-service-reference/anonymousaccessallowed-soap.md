---
title: AnonymousAccessAllowed (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: bf819a65-30f2-4881-a34f-cb30a9c2b6a7
description: O elemento AnonymousAccessAllowed indica se um local de compartilhamento de documentos requer um usuário autenticado.
ms.openlocfilehash: b3ff22fbba603bbd74dc08a0dbb1d8687714fe7d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466077"
---
# <a name="anonymousaccessallowed-soap"></a><span data-ttu-id="6474b-103">AnonymousAccessAllowed (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6474b-103">AnonymousAccessAllowed (SOAP)</span></span>

<span data-ttu-id="6474b-104">O elemento **AnonymousAccessAllowed** indica se um local de compartilhamento de documentos requer um usuário autenticado.</span><span class="sxs-lookup"><span data-stu-id="6474b-104">The **AnonymousAccessAllowed** element indicates whether a document sharing location requires an authenticated user.</span></span> 
  
```XML
<AnonymousAccessAllowed /> 
```

 <span data-ttu-id="6474b-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="6474b-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6474b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6474b-106">Attributes and elements</span></span>

<span data-ttu-id="6474b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6474b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6474b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6474b-108">Attributes</span></span>

<span data-ttu-id="6474b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6474b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6474b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6474b-110">Child elements</span></span>

<span data-ttu-id="6474b-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6474b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6474b-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6474b-112">Parent elements</span></span>

|<span data-ttu-id="6474b-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6474b-113">**Element**</span></span>|<span data-ttu-id="6474b-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6474b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6474b-115">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6474b-115">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="6474b-116">Representa informações de localização e metadados de um local de compartilhamento de documentos.</span><span class="sxs-lookup"><span data-stu-id="6474b-116">Represents location and metadata information for a document sharing location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6474b-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="6474b-117">Text value</span></span>

<span data-ttu-id="6474b-118">O valor booliano do elemento **AnonymousAccessAllowed** indica se o local de compartilhamento requer um usuário autenticado.</span><span class="sxs-lookup"><span data-stu-id="6474b-118">The Boolean value of the **AnonymousAccessAllowed** element indicates whether the sharing location requires an authenticated user.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="6474b-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6474b-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6474b-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="6474b-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="6474b-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6474b-121">Schema Name</span></span>  <br/> |<span data-ttu-id="6474b-122">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="6474b-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="6474b-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6474b-123">Validation File</span></span>  <br/> |<span data-ttu-id="6474b-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6474b-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6474b-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6474b-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="6474b-126">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="6474b-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6474b-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="6474b-127">See also</span></span>

- [<span data-ttu-id="6474b-128">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6474b-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="6474b-129">Referência do serviço Web de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="6474b-129">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="6474b-130">Elementos XML de descoberta automática SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="6474b-130">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

