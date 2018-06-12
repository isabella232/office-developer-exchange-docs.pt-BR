---
title: ResponseCode (InvalidRecipientResponseCodeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 582e9caa-d2bc-4be1-a460-739294f9ef18
description: O elemento ResponseCode fornece informações sobre por que o destinatário é inválido.
ms.openlocfilehash: 3bff99dd1ac6603ce31d5ceb074e73ef48190bb2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825186"
---
# <a name="responsecode-invalidrecipientresponsecodetype"></a><span data-ttu-id="31ce9-103">ResponseCode (InvalidRecipientResponseCodeType)</span><span class="sxs-lookup"><span data-stu-id="31ce9-103">ResponseCode (InvalidRecipientResponseCodeType)</span></span>

<span data-ttu-id="31ce9-104">O elemento **ResponseCode** fornece informações sobre por que o destinatário é inválido.</span><span class="sxs-lookup"><span data-stu-id="31ce9-104">The **ResponseCode** element provides information about why the recipient is invalid.</span></span> 
  
```XML
<ResponseCode>OtherError or RecipientOrganizationNotFederated or CannotObtainTokenFromSTS or SystemPolicyBlocksSharingWithThisRecipient or RecipientOrganizationFederatedWithUnknownTokenIssuer</ResponseCode>
```

 <span data-ttu-id="31ce9-105">**InvalidRecipientResponseCodeType**</span><span class="sxs-lookup"><span data-stu-id="31ce9-105">**InvalidRecipientResponseCodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31ce9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="31ce9-106">Attributes and elements</span></span>

<span data-ttu-id="31ce9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="31ce9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31ce9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="31ce9-108">Attributes</span></span>

<span data-ttu-id="31ce9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="31ce9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="31ce9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="31ce9-110">Child elements</span></span>

<span data-ttu-id="31ce9-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="31ce9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="31ce9-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="31ce9-112">Parent elements</span></span>

|<span data-ttu-id="31ce9-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="31ce9-113">**Element**</span></span>|<span data-ttu-id="31ce9-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="31ce9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31ce9-115">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="31ce9-115">InvalidRecipient</span></span>](invalidrecipient.md) <br/> |<span data-ttu-id="31ce9-116">Contém o endereço SMTP do destinatário inválido e informações sobre por que o destinatário é inválido.</span><span class="sxs-lookup"><span data-stu-id="31ce9-116">Contains the SMTP address of the invalid recipient and information about why the recipient is invalid.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="31ce9-117">Text value</span><span class="sxs-lookup"><span data-stu-id="31ce9-117">Text value</span></span>

<span data-ttu-id="31ce9-118">A tabela a seguir lista os valores possíveis para o elemento **ResponseCode** .</span><span class="sxs-lookup"><span data-stu-id="31ce9-118">The following table lists the possible values for the **ResponseCode** element.</span></span> 
  
|<span data-ttu-id="31ce9-119">**Code**</span><span class="sxs-lookup"><span data-stu-id="31ce9-119">**Code**</span></span>|<span data-ttu-id="31ce9-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="31ce9-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="31ce9-121">OtherError</span><span class="sxs-lookup"><span data-stu-id="31ce9-121">OtherError</span></span>  <br/> |<span data-ttu-id="31ce9-122">Indica que o erro não for especificado por outro código de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="31ce9-122">Indicates that the error is not specified by another error response code.</span></span>  <br/> |
|<span data-ttu-id="31ce9-123">RecipientOrganizationNotFederated</span><span class="sxs-lookup"><span data-stu-id="31ce9-123">RecipientOrganizationNotFederated</span></span>  <br/> |<span data-ttu-id="31ce9-124">Indica que uma relação de compartilhamento não está disponível com a organização especificada no endereço de email SMTP do destinatário.</span><span class="sxs-lookup"><span data-stu-id="31ce9-124">Indicates that a sharing relationship is not available with the organization specified in the recipient's SMTP e-mail address.</span></span>  <br/> |
|<span data-ttu-id="31ce9-125">CannotObtainTokenFromSTS</span><span class="sxs-lookup"><span data-stu-id="31ce9-125">CannotObtainTokenFromSTS</span></span>  <br/> |<span data-ttu-id="31ce9-126">Indica que houve um problema ao obter um token de segurança do servidor de token.</span><span class="sxs-lookup"><span data-stu-id="31ce9-126">Indicates that there was a problem obtaining a security token from the token server.</span></span>  <br/> |
|<span data-ttu-id="31ce9-127">SystemPolicyBlocksSharingWithThisRecipient</span><span class="sxs-lookup"><span data-stu-id="31ce9-127">SystemPolicyBlocksSharingWithThisRecipient</span></span>  <br/> |<span data-ttu-id="31ce9-128">Indica que o administrador do sistema tiver definido uma diretiva de sistema que bloqueia o compartilhamento com o destinatário especificado.</span><span class="sxs-lookup"><span data-stu-id="31ce9-128">Indicates that the system administrator has set a system policy that blocks sharing with the specified recipient.</span></span>  <br/> |
|<span data-ttu-id="31ce9-129">RecipientOrganizationFederatedWithUnknownTokenIssuer</span><span class="sxs-lookup"><span data-stu-id="31ce9-129">RecipientOrganizationFederatedWithUnknownTokenIssuer</span></span>  <br/> |<span data-ttu-id="31ce9-130">Indica que o serviço de token seguro que é usado pelo destinatário especificado é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="31ce9-130">Indicates that the secure token service that is used by the specified recipient is unknown.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="31ce9-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="31ce9-131">Remarks</span></span>

<span data-ttu-id="31ce9-132">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="31ce9-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="31ce9-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="31ce9-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31ce9-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="31ce9-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="31ce9-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="31ce9-135">Schema Name</span></span>  <br/> |<span data-ttu-id="31ce9-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="31ce9-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="31ce9-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="31ce9-137">Validation File</span></span>  <br/> |<span data-ttu-id="31ce9-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="31ce9-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="31ce9-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="31ce9-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="31ce9-140">False</span><span class="sxs-lookup"><span data-stu-id="31ce9-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="31ce9-141">Ver também</span><span class="sxs-lookup"><span data-stu-id="31ce9-141">See also</span></span>



[<span data-ttu-id="31ce9-142">Operação GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="31ce9-142">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="31ce9-143">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="31ce9-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

