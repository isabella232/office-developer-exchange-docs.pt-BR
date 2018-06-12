---
title: SupportedFileExtensions (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 6f73d18c-7bb1-4ab6-a23b-6d948e590b53
description: O elemento SupportedFileExtensions lista as extensões de arquivo que podem ser armazenadas em um local de compartilhamento de documento.
ms.openlocfilehash: 0f1dbbce2b836fe05e4bc612c607302783d5e05d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837677"
---
# <a name="supportedfileextensions-soap"></a><span data-ttu-id="30a05-103">SupportedFileExtensions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="30a05-103">SupportedFileExtensions (SOAP)</span></span>

<span data-ttu-id="30a05-104">O elemento **SupportedFileExtensions** lista as extensões de arquivo que podem ser armazenadas em um local de compartilhamento de documento.</span><span class="sxs-lookup"><span data-stu-id="30a05-104">The **SupportedFileExtensions** element lists the file extensions that can be stored in a document sharing location.</span></span> 
  
```XML
<SupportedFileExtensions /> 
```

 <span data-ttu-id="30a05-105">**ArrayOfFileExtension**</span><span class="sxs-lookup"><span data-stu-id="30a05-105">**ArrayOfFileExtension**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="30a05-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="30a05-106">Attributes and elements</span></span>

<span data-ttu-id="30a05-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="30a05-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30a05-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="30a05-108">Attributes</span></span>

<span data-ttu-id="30a05-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="30a05-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="30a05-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="30a05-110">Child elements</span></span>

|<span data-ttu-id="30a05-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="30a05-111">**Element**</span></span>|<span data-ttu-id="30a05-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="30a05-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30a05-113">FileExtension (SOAP)</span><span class="sxs-lookup"><span data-stu-id="30a05-113">FileExtension (SOAP)</span></span>](fileextension-soap.md) <br/> |<span data-ttu-id="30a05-114">Representa uma extensão de arquivo.</span><span class="sxs-lookup"><span data-stu-id="30a05-114">Represents a file extension.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="30a05-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="30a05-115">Parent elements</span></span>

|<span data-ttu-id="30a05-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="30a05-116">**Element**</span></span>|<span data-ttu-id="30a05-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="30a05-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30a05-118">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="30a05-118">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="30a05-119">Representa informações de local e metadados para um local de compartilhamento de documentos.</span><span class="sxs-lookup"><span data-stu-id="30a05-119">Represents location and metadata information for a document sharing location.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="30a05-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="30a05-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30a05-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="30a05-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="30a05-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="30a05-122">Schema Name</span></span>  <br/> |<span data-ttu-id="30a05-123">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="30a05-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="30a05-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="30a05-124">Validation File</span></span>  <br/> |<span data-ttu-id="30a05-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="30a05-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="30a05-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="30a05-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="30a05-127">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="30a05-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="30a05-128">Ver também</span><span class="sxs-lookup"><span data-stu-id="30a05-128">See also</span></span>



[<span data-ttu-id="30a05-129">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="30a05-129">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="30a05-130">Referência de web service de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="30a05-130">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="30a05-131">Elementos de Autodiscover XML SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="30a05-131">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

