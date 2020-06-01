---
title: DocumentSharingLocation (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 21bc388c-33be-422b-a89d-30ade0fae8f1
description: O elemento DocumentSharingLocation contém informações de local e metadados de um local de compartilhamento de documentos.
ms.openlocfilehash: 6fed933da979ab3e3fca51ba606127b7f0a4e3f8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457057"
---
# <a name="documentsharinglocation-soap"></a><span data-ttu-id="9ce2e-103">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ce2e-103">DocumentSharingLocation (SOAP)</span></span>

<span data-ttu-id="9ce2e-104">O elemento **DocumentSharingLocation** contém informações de local e metadados de um local de compartilhamento de documentos.</span><span class="sxs-lookup"><span data-stu-id="9ce2e-104">The **DocumentSharingLocation** element contains location and metadata information for a document sharing location.</span></span> 
  
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

 <span data-ttu-id="9ce2e-105">**DocumentSharingLocation**</span><span class="sxs-lookup"><span data-stu-id="9ce2e-105">**DocumentSharingLocation**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9ce2e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9ce2e-106">Attributes and elements</span></span>

<span data-ttu-id="9ce2e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9ce2e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ce2e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9ce2e-108">Attributes</span></span>

<span data-ttu-id="9ce2e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9ce2e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ce2e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9ce2e-110">Child elements</span></span>

|<span data-ttu-id="9ce2e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9ce2e-111">**Element**</span></span>|<span data-ttu-id="9ce2e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9ce2e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ce2e-113">ServiceUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ce2e-113">ServiceUrl (SOAP)</span></span>](serviceurl-soap.md) <br/> |<span data-ttu-id="9ce2e-114">Representa a URL do serviço Web de compartilhamento de documentos.</span><span class="sxs-lookup"><span data-stu-id="9ce2e-114">Represents the URL of the document sharing web service.</span></span>  <br/> |
|[<span data-ttu-id="9ce2e-115">LocationUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ce2e-115">LocationUrl (SOAP)</span></span>](locationurl-soap.md) <br/> |<span data-ttu-id="9ce2e-116">Representa a URL do local de compartilhamento de documentos.</span><span class="sxs-lookup"><span data-stu-id="9ce2e-116">Represents the URL of the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="9ce2e-117">DisplayName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ce2e-117">DisplayName (SOAP)</span></span>](displayname-soap.md) <br/> |<span data-ttu-id="9ce2e-118">Representa o nome do local de compartilhamento de documento a ser usado na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="9ce2e-118">Represents the name of the document sharing location to use in the UI.</span></span>  <br/> |
|[<span data-ttu-id="9ce2e-119">SupportedFileExtensions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ce2e-119">SupportedFileExtensions (SOAP)</span></span>](supportedfileextensions-soap.md) <br/> |<span data-ttu-id="9ce2e-120">Representa as extensões de arquivo que podem ser armazenadas no local de compartilhamento de documentos.</span><span class="sxs-lookup"><span data-stu-id="9ce2e-120">Represents the file extensions that can be stored in the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="9ce2e-121">ExternalAccessAllowed (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ce2e-121">ExternalAccessAllowed (SOAP)</span></span>](externalaccessallowed-soap.md) <br/> |<span data-ttu-id="9ce2e-122">Indica se o local de compartilhamento de documento está disponível para conexões externas.</span><span class="sxs-lookup"><span data-stu-id="9ce2e-122">Indicates whether the document sharing location is available to outside connections.</span></span>  <br/> |
|[<span data-ttu-id="9ce2e-123">AnonymousAccessAllowed (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ce2e-123">AnonymousAccessAllowed (SOAP)</span></span>](anonymousaccessallowed-soap.md) <br/> |<span data-ttu-id="9ce2e-124">Indica se o acesso ao local de compartilhamento requer um usuário autenticado.</span><span class="sxs-lookup"><span data-stu-id="9ce2e-124">Indicates whether access to the sharing location requires an authenticated user.</span></span>  <br/> |
|[<span data-ttu-id="9ce2e-125">CanModifyPermissions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ce2e-125">CanModifyPermissions (SOAP)</span></span>](canmodifypermissions-soap.md) <br/> |<span data-ttu-id="9ce2e-126">Indica se o usuário pode modificar permissões de acesso para o local de compartilhamento de documentos.</span><span class="sxs-lookup"><span data-stu-id="9ce2e-126">Indicates whether the user can modify access permissions to the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="9ce2e-127">IsDefault (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ce2e-127">IsDefault (SOAP)</span></span>](isdefault-soap.md) <br/> |<span data-ttu-id="9ce2e-128">Indica se o local de compartilhamento de documento é o local de compartilhamento padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="9ce2e-128">Indicates whether the document sharing location is the user's default sharing location.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9ce2e-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9ce2e-129">Parent elements</span></span>

|<span data-ttu-id="9ce2e-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9ce2e-130">**Element**</span></span>|<span data-ttu-id="9ce2e-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9ce2e-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ce2e-132">DocumentSharingLocations (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ce2e-132">DocumentSharingLocations (SOAP)</span></span>](documentsharinglocations-soap.md) <br/> |<span data-ttu-id="9ce2e-133">Contém uma lista de locais e metadados de compartilhamento de documentos.</span><span class="sxs-lookup"><span data-stu-id="9ce2e-133">Contains a list of document sharing locations and metadata.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9ce2e-134">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="9ce2e-134">Text value</span></span>

<span data-ttu-id="9ce2e-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9ce2e-135">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ce2e-136">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9ce2e-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ce2e-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="9ce2e-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="9ce2e-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9ce2e-138">Schema Name</span></span>  <br/> |<span data-ttu-id="9ce2e-139">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="9ce2e-139">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="9ce2e-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9ce2e-140">Validation File</span></span>  <br/> |<span data-ttu-id="9ce2e-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9ce2e-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9ce2e-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9ce2e-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="9ce2e-143">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="9ce2e-143">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ce2e-144">Também consulte</span><span class="sxs-lookup"><span data-stu-id="9ce2e-144">See also</span></span>

- [<span data-ttu-id="9ce2e-145">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ce2e-145">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="9ce2e-146">Referência do serviço Web de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="9ce2e-146">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="9ce2e-147">Elementos XML de descoberta automática SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="9ce2e-147">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

