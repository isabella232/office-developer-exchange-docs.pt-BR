---
title: DocumentSharingLocation (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 21bc388c-33be-422b-a89d-30ade0fae8f1
description: O elemento DocumentSharingLocation contém informações de metadados para um local de compartilhamento de documentos e local.
ms.openlocfilehash: d258efecb46d570138c7c2c78ed9d2fa9a275103
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751908"
---
# <a name="documentsharinglocation-soap"></a><span data-ttu-id="0b1d1-103">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0b1d1-103">DocumentSharingLocation (SOAP)</span></span>

<span data-ttu-id="0b1d1-104">O elemento **DocumentSharingLocation** contém informações de metadados para um local de compartilhamento de documentos e local.</span><span class="sxs-lookup"><span data-stu-id="0b1d1-104">The **DocumentSharingLocation** element contains location and metadata information for a document sharing location.</span></span> 
  
```XML
<DocumentSharingLocation>
   <ServiceUrl />
   <LocationUrl />
   <DisplayName />
   <SupportedFileExtensions />
   <ExternalAccessAllowed />
   <AnonymousAccessAllowed />
   <CanModifyPermissions />
   <IsDefault />
</DocumentSharingLocation>
```

 <span data-ttu-id="0b1d1-105">**DocumentSharingLocation**</span><span class="sxs-lookup"><span data-stu-id="0b1d1-105">**DocumentSharingLocation**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b1d1-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0b1d1-106">Attributes and elements</span></span>

<span data-ttu-id="0b1d1-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0b1d1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b1d1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0b1d1-108">Attributes</span></span>

<span data-ttu-id="0b1d1-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0b1d1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0b1d1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0b1d1-110">Child elements</span></span>

|<span data-ttu-id="0b1d1-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0b1d1-111">**Element**</span></span>|<span data-ttu-id="0b1d1-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0b1d1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b1d1-113">ServiceUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0b1d1-113">ServiceUrl (SOAP)</span></span>](serviceurl-soap.md) <br/> |<span data-ttu-id="0b1d1-114">Representa a URL do documento compartilhamento de serviço web.</span><span class="sxs-lookup"><span data-stu-id="0b1d1-114">Represents the URL of the document sharing web service.</span></span>  <br/> |
|[<span data-ttu-id="0b1d1-115">LocationUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0b1d1-115">LocationUrl (SOAP)</span></span>](locationurl-soap.md) <br/> |<span data-ttu-id="0b1d1-116">Representa a URL do documento local de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="0b1d1-116">Represents the URL of the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="0b1d1-117">DisplayName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0b1d1-117">DisplayName (SOAP)</span></span>](displayname-soap.md) <br/> |<span data-ttu-id="0b1d1-118">Representa o nome do documento compartilhamento local a ser usado na interface de usuário.</span><span class="sxs-lookup"><span data-stu-id="0b1d1-118">Represents the name of the document sharing location to use in the UI.</span></span>  <br/> |
|[<span data-ttu-id="0b1d1-119">SupportedFileExtensions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0b1d1-119">SupportedFileExtensions (SOAP)</span></span>](supportedfileextensions-soap.md) <br/> |<span data-ttu-id="0b1d1-120">Representa as extensões de arquivo que podem ser armazenadas no documento local de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="0b1d1-120">Represents the file extensions that can be stored in the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="0b1d1-121">ExternalAccessAllowed (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0b1d1-121">ExternalAccessAllowed (SOAP)</span></span>](externalaccessallowed-soap.md) <br/> |<span data-ttu-id="0b1d1-122">Indica se o documento local de compartilhamento está disponível para fora de conexões.</span><span class="sxs-lookup"><span data-stu-id="0b1d1-122">Indicates whether the document sharing location is available to outside connections.</span></span>  <br/> |
|[<span data-ttu-id="0b1d1-123">AnonymousAccessAllowed (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0b1d1-123">AnonymousAccessAllowed (SOAP)</span></span>](anonymousaccessallowed-soap.md) <br/> |<span data-ttu-id="0b1d1-124">Indica se o acesso à localização de compartilhamento requer um usuário autenticado.</span><span class="sxs-lookup"><span data-stu-id="0b1d1-124">Indicates whether access to the sharing location requires an authenticated user.</span></span>  <br/> |
|[<span data-ttu-id="0b1d1-125">CanModifyPermissions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0b1d1-125">CanModifyPermissions (SOAP)</span></span>](canmodifypermissions-soap.md) <br/> |<span data-ttu-id="0b1d1-126">Indica se o usuário pode modificar permissões de acesso para o documento local de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="0b1d1-126">Indicates whether the user can modify access permissions to the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="0b1d1-127">IsDefault (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0b1d1-127">IsDefault (SOAP)</span></span>](isdefault-soap.md) <br/> |<span data-ttu-id="0b1d1-128">Indica se o documento local de compartilhamento é o padrão do usuário local de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="0b1d1-128">Indicates whether the document sharing location is the user's default sharing location.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0b1d1-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0b1d1-129">Parent elements</span></span>

|<span data-ttu-id="0b1d1-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0b1d1-130">**Element**</span></span>|<span data-ttu-id="0b1d1-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0b1d1-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b1d1-132">DocumentSharingLocations (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0b1d1-132">DocumentSharingLocations (SOAP)</span></span>](documentsharinglocations-soap.md) <br/> |<span data-ttu-id="0b1d1-133">Contém uma lista de locais e metadados de compartilhamento de documentos.</span><span class="sxs-lookup"><span data-stu-id="0b1d1-133">Contains a list of document sharing locations and metadata.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0b1d1-134">Text value</span><span class="sxs-lookup"><span data-stu-id="0b1d1-134">Text value</span></span>

<span data-ttu-id="0b1d1-135">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0b1d1-135">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b1d1-136">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0b1d1-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b1d1-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="0b1d1-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="0b1d1-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0b1d1-138">Schema Name</span></span>  <br/> |<span data-ttu-id="0b1d1-139">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="0b1d1-139">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="0b1d1-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0b1d1-140">Validation File</span></span>  <br/> |<span data-ttu-id="0b1d1-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0b1d1-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0b1d1-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0b1d1-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="0b1d1-143">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="0b1d1-143">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b1d1-144">Ver também</span><span class="sxs-lookup"><span data-stu-id="0b1d1-144">See also</span></span>

- [<span data-ttu-id="0b1d1-145">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0b1d1-145">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="0b1d1-146">Referência de web service de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="0b1d1-146">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="0b1d1-147">Elementos de Autodiscover XML SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0b1d1-147">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

