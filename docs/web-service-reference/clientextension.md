---
title: ClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3445ef2b-1bb1-43ea-bc93-85c72401e5b6
description: O elemento ClientExtension contém informações de usuário e de configuração sobre um aplicativo.
ms.openlocfilehash: 5051248a2c8e664d82666bd7b42ee3c3046f43fe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751394"
---
# <a name="clientextension"></a><span data-ttu-id="25507-103">ClientExtension</span><span class="sxs-lookup"><span data-stu-id="25507-103">ClientExtension</span></span>

<span data-ttu-id="25507-104">O elemento **ClientExtension** contém informações de usuário e de configuração sobre um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="25507-104">The **ClientExtension** element contains user and configuration information about an app.</span></span> 
  
```XML
<ClientExtension IsAvailable=" true | false " IsMandatory=" true | false " IsEnabledByDefault=" true | false " Type="" Scope="" MarketplaceAssetId="" MarketplaceContentMarket="" AppStatus="" Etoken="">
    <SpecificUsers></SpecificUsers>
    <Manifest></Manifest>
</ClientExtension>
```

 <span data-ttu-id="25507-105">**ClientExtensionType**</span><span class="sxs-lookup"><span data-stu-id="25507-105">**ClientExtensionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="25507-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="25507-106">Attributes and elements</span></span>

<span data-ttu-id="25507-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="25507-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25507-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="25507-108">Attributes</span></span>

|<span data-ttu-id="25507-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="25507-109">**Attribute**</span></span>|<span data-ttu-id="25507-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="25507-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="25507-111">IsAvailable</span><span class="sxs-lookup"><span data-stu-id="25507-111">IsAvailable</span></span>  <br/> |<span data-ttu-id="25507-112">Especifica se o aplicativo está disponível.</span><span class="sxs-lookup"><span data-stu-id="25507-112">Specifies whether the app is available.</span></span> <span data-ttu-id="25507-113">Um valor de **true** para o atributo **IsAvailable** text indica que o aplicativo está disponível.</span><span class="sxs-lookup"><span data-stu-id="25507-113">A text value of **true** for the **IsAvailable** attribute indicates that the app is available.</span></span> <span data-ttu-id="25507-114">Um valor **false** indica que o aplicativo não está disponível.</span><span class="sxs-lookup"><span data-stu-id="25507-114">A value of **false** indicates that the app is not available.</span></span> <span data-ttu-id="25507-115">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="25507-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="25507-116">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="25507-116">IsMandatory</span></span>  <br/> |<span data-ttu-id="25507-117">Especifica se o aplicativo é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25507-117">Specifies whether the app is mandatory.</span></span> <span data-ttu-id="25507-118">Um valor de texto de **true** para o atributo **IsMandatory** indica que o aplicativo é obrigatório para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="25507-118">A text value of **true** for the **IsMandatory** attribute indicates that the app is mandatory for the mailbox.</span></span> <span data-ttu-id="25507-119">Um valor **false** indica que o aplicativo não é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25507-119">A value of **false** indicates that the app is not mandatory.</span></span> <span data-ttu-id="25507-120">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="25507-120">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="25507-121">IsEnabledByDefault</span><span class="sxs-lookup"><span data-stu-id="25507-121">IsEnabledByDefault</span></span>  <br/> |<span data-ttu-id="25507-122">Especifica se o aplicativo está habilitado por padrão.</span><span class="sxs-lookup"><span data-stu-id="25507-122">Specifies whether the app is enabled by default.</span></span> <span data-ttu-id="25507-123">Um valor de texto de **true** para o atributo **IsEnabledByDefault** indica que o aplicativo está habilitado por padrão.</span><span class="sxs-lookup"><span data-stu-id="25507-123">A text value of **true** for the **IsEnabledByDefault** attribute indicates that the app is enabled by default.</span></span> <span data-ttu-id="25507-124">Um valor **false** indica que o aplicativo não está ativado por padrão.</span><span class="sxs-lookup"><span data-stu-id="25507-124">A value of **false** indicates that the app is not enabled by default.</span></span> <span data-ttu-id="25507-125">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="25507-125">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="25507-126">ProvidedTo</span><span class="sxs-lookup"><span data-stu-id="25507-126">ProvidedTo</span></span>  <br/> |<span data-ttu-id="25507-127">Especifica a qual o aplicativo é fornecido.</span><span class="sxs-lookup"><span data-stu-id="25507-127">Specifies to whom the app is provided.</span></span> <span data-ttu-id="25507-128">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="25507-128">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="25507-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="25507-129">Type</span></span>  <br/> |<span data-ttu-id="25507-130">Especifica o tipo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="25507-130">Specifies the type of the app.</span></span>  <br/> |
|<span data-ttu-id="25507-131">Escopo</span><span class="sxs-lookup"><span data-stu-id="25507-131">Scope</span></span>  <br/> |<span data-ttu-id="25507-132">Especifica o escopo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="25507-132">Specifies the scope of the app.</span></span>  <br/> |
|<span data-ttu-id="25507-133">MarketplaceAssetId</span><span class="sxs-lookup"><span data-stu-id="25507-133">MarketplaceAssetId</span></span>  <br/> |<span data-ttu-id="25507-134">Especifica o identificador de ativos do marketplace do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="25507-134">Specifies the marketplace asset identifier of the app.</span></span>  <br/> |
|<span data-ttu-id="25507-135">MarketplaceContentMarket</span><span class="sxs-lookup"><span data-stu-id="25507-135">MarketplaceContentMarket</span></span>  <br/> |<span data-ttu-id="25507-136">Especifica o conteúdo do marketplace que um usuário vê para obter detalhes e analisa sobre um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="25507-136">Specifies the marketplace content that a user sees for details and reviews about an app.</span></span>  <br/> |
|<span data-ttu-id="25507-137">AppStatus</span><span class="sxs-lookup"><span data-stu-id="25507-137">AppStatus</span></span>  <br/> |<span data-ttu-id="25507-138">Especifica o código de status de um aplicativo de email em um estado inesperado.</span><span class="sxs-lookup"><span data-stu-id="25507-138">Specifies the status code of a mail app in an unexpected state.</span></span>  <br/> |
|<span data-ttu-id="25507-139">Etoken</span><span class="sxs-lookup"><span data-stu-id="25507-139">Etoken</span></span>  <br/> |<span data-ttu-id="25507-140">Especifica o token de licença para aplicativos de email paga ou de avaliação.</span><span class="sxs-lookup"><span data-stu-id="25507-140">Specifies the license token for paid or trial mail apps.</span></span>  <br/> |
   
#### <a name="type"></a><span data-ttu-id="25507-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="25507-141">Type</span></span>

|<span data-ttu-id="25507-142">**Valor**</span><span class="sxs-lookup"><span data-stu-id="25507-142">**Value**</span></span>|<span data-ttu-id="25507-143">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="25507-143">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="25507-144">Default</span><span class="sxs-lookup"><span data-stu-id="25507-144">Default</span></span>  <br/> |<span data-ttu-id="25507-145">Indica que o aplicativo está disponível por padrão.</span><span class="sxs-lookup"><span data-stu-id="25507-145">Indicates that the app is available by default.</span></span>  <br/> |
|<span data-ttu-id="25507-146">Particular</span><span class="sxs-lookup"><span data-stu-id="25507-146">Private</span></span>  <br/> |<span data-ttu-id="25507-147">Indica que o aplicativo é privado.</span><span class="sxs-lookup"><span data-stu-id="25507-147">Indicates that the app is private.</span></span>  <br/> |
|<span data-ttu-id="25507-148">MarketPlace</span><span class="sxs-lookup"><span data-stu-id="25507-148">MarketPlace</span></span>  <br/> |<span data-ttu-id="25507-149">Indica que o aplicativo é um aplicativo do marketplace.</span><span class="sxs-lookup"><span data-stu-id="25507-149">Indicates that the app is a marketplace app.</span></span>  <br/> |
   
#### <a name="scope"></a><span data-ttu-id="25507-150">Escopo</span><span class="sxs-lookup"><span data-stu-id="25507-150">Scope</span></span>

|<span data-ttu-id="25507-151">**Valor**</span><span class="sxs-lookup"><span data-stu-id="25507-151">**Value**</span></span>|<span data-ttu-id="25507-152">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="25507-152">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="25507-153">None</span><span class="sxs-lookup"><span data-stu-id="25507-153">None</span></span>  <br/> |<span data-ttu-id="25507-154">Indica que o aplicativo não tem nenhum escopo.</span><span class="sxs-lookup"><span data-stu-id="25507-154">Indicates that the app has no scope.</span></span>  <br/> |
|<span data-ttu-id="25507-155">Usuário</span><span class="sxs-lookup"><span data-stu-id="25507-155">User</span></span>  <br/> |<span data-ttu-id="25507-156">Indica que o aplicativo é por usuário.</span><span class="sxs-lookup"><span data-stu-id="25507-156">Indicates that the app is per user.</span></span>  <br/> |
|<span data-ttu-id="25507-157">Organização</span><span class="sxs-lookup"><span data-stu-id="25507-157">Organization</span></span>  <br/> |<span data-ttu-id="25507-158">Indica que o aplicativo é para uma organização.</span><span class="sxs-lookup"><span data-stu-id="25507-158">Indicates that the app is for an organization.</span></span>  <br/> |
|<span data-ttu-id="25507-159">Default</span><span class="sxs-lookup"><span data-stu-id="25507-159">Default</span></span>  <br/> |<span data-ttu-id="25507-160">Indica que o aplicativo é um aplicativo padrão.</span><span class="sxs-lookup"><span data-stu-id="25507-160">Indicates that the app is a default app.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="25507-161">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="25507-161">Child elements</span></span>

|<span data-ttu-id="25507-162">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="25507-162">**Element**</span></span>|<span data-ttu-id="25507-163">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="25507-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25507-164">SpecificUsers</span><span class="sxs-lookup"><span data-stu-id="25507-164">SpecificUsers</span></span>](specificusers.md) <br/> |<span data-ttu-id="25507-165">Especifica as contas de email que podem acessar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="25507-165">Specifies the email accounts that can access the app.</span></span>  <br/> |
|[<span data-ttu-id="25507-166">Manifesto</span><span class="sxs-lookup"><span data-stu-id="25507-166">Manifest</span></span>](manifest.md) <br/> |<span data-ttu-id="25507-167">Contém o arquivo de manifesto do aplicativo codificada de base 64.</span><span class="sxs-lookup"><span data-stu-id="25507-167">Contains the base-64 encoded app manifest file.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="25507-168">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="25507-168">Parent elements</span></span>

|<span data-ttu-id="25507-169">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="25507-169">**Element**</span></span>|<span data-ttu-id="25507-170">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="25507-170">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25507-171">ClientExtensions</span><span class="sxs-lookup"><span data-stu-id="25507-171">ClientExtensions</span></span>](clientextensions.md) <br/> |<span data-ttu-id="25507-172">Especifica uma matriz de elementos de **ClientExtension** .</span><span class="sxs-lookup"><span data-stu-id="25507-172">Specifies an array of **ClientExtension** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="25507-173">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="25507-173">Remarks</span></span>

<span data-ttu-id="25507-174">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="25507-174">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="25507-175">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="25507-175">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25507-176">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="25507-176">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25507-177">Namespace</span><span class="sxs-lookup"><span data-stu-id="25507-177">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="25507-178">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="25507-178">Schema Name</span></span>  <br/> |<span data-ttu-id="25507-179">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="25507-179">Type schema</span></span>  <br/> |
|<span data-ttu-id="25507-180">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="25507-180">Validation File</span></span>  <br/> |<span data-ttu-id="25507-181">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="25507-181">types.xsd</span></span>  <br/> |
|<span data-ttu-id="25507-182">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="25507-182">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="25507-183">Confira também</span><span class="sxs-lookup"><span data-stu-id="25507-183">See also</span></span>



- [<span data-ttu-id="25507-184">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="25507-184">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

