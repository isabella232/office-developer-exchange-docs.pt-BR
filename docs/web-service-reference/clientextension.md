---
title: ClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3445ef2b-1bb1-43ea-bc93-85c72401e5b6
description: O elemento ClientExtension contém informações de usuário e configuração sobre um aplicativo.
ms.openlocfilehash: d3d9ce1d242a63f28da3464f0faff86abde502c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460194"
---
# <a name="clientextension"></a><span data-ttu-id="e7f1b-103">ClientExtension</span><span class="sxs-lookup"><span data-stu-id="e7f1b-103">ClientExtension</span></span>

<span data-ttu-id="e7f1b-104">O elemento **ClientExtension** contém informações de usuário e configuração sobre um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-104">The **ClientExtension** element contains user and configuration information about an app.</span></span> 
  
```XML
<ClientExtension IsAvailable=" true | false " IsMandatory=" true | false " IsEnabledByDefault=" true | false " Type="" Scope="" MarketplaceAssetId="" MarketplaceContentMarket="" AppStatus="" Etoken="">
    <SpecificUsers></SpecificUsers>
    <Manifest></Manifest>
</ClientExtension>
```

 <span data-ttu-id="e7f1b-105">**ClientExtensionType**</span><span class="sxs-lookup"><span data-stu-id="e7f1b-105">**ClientExtensionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e7f1b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e7f1b-106">Attributes and elements</span></span>

<span data-ttu-id="e7f1b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7f1b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e7f1b-108">Attributes</span></span>

|<span data-ttu-id="e7f1b-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="e7f1b-109">**Attribute**</span></span>|<span data-ttu-id="e7f1b-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e7f1b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e7f1b-111">IsAvailable</span><span class="sxs-lookup"><span data-stu-id="e7f1b-111">IsAvailable</span></span>  <br/> |<span data-ttu-id="e7f1b-112">Especifica se o aplicativo está disponível.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-112">Specifies whether the app is available.</span></span> <span data-ttu-id="e7f1b-113">Um valor de texto **true** para o atributo **IsAvailable** indica que o aplicativo está disponível.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-113">A text value of **true** for the **IsAvailable** attribute indicates that the app is available.</span></span> <span data-ttu-id="e7f1b-114">Um valor **false** indica que o aplicativo não está disponível.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-114">A value of **false** indicates that the app is not available.</span></span> <span data-ttu-id="e7f1b-115">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="e7f1b-116">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="e7f1b-116">IsMandatory</span></span>  <br/> |<span data-ttu-id="e7f1b-117">Especifica se o aplicativo é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-117">Specifies whether the app is mandatory.</span></span> <span data-ttu-id="e7f1b-118">Um valor de texto **true** para o atributo **IsMandatory** indica que o aplicativo é obrigatório para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-118">A text value of **true** for the **IsMandatory** attribute indicates that the app is mandatory for the mailbox.</span></span> <span data-ttu-id="e7f1b-119">Um valor **false** indica que o aplicativo não é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-119">A value of **false** indicates that the app is not mandatory.</span></span> <span data-ttu-id="e7f1b-120">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-120">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="e7f1b-121">IsEnabledByDefault</span><span class="sxs-lookup"><span data-stu-id="e7f1b-121">IsEnabledByDefault</span></span>  <br/> |<span data-ttu-id="e7f1b-122">Especifica se o aplicativo está habilitado por padrão.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-122">Specifies whether the app is enabled by default.</span></span> <span data-ttu-id="e7f1b-123">Um valor de texto **true** para o atributo **IsEnabledByDefault** indica que o aplicativo está habilitado por padrão.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-123">A text value of **true** for the **IsEnabledByDefault** attribute indicates that the app is enabled by default.</span></span> <span data-ttu-id="e7f1b-124">Um valor **false** indica que o aplicativo não está habilitado por padrão.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-124">A value of **false** indicates that the app is not enabled by default.</span></span> <span data-ttu-id="e7f1b-125">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-125">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="e7f1b-126">ProvidedTo</span><span class="sxs-lookup"><span data-stu-id="e7f1b-126">ProvidedTo</span></span>  <br/> |<span data-ttu-id="e7f1b-127">Especifica para quem o aplicativo é fornecido.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-127">Specifies to whom the app is provided.</span></span> <span data-ttu-id="e7f1b-128">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-128">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="e7f1b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7f1b-129">Type</span></span>  <br/> |<span data-ttu-id="e7f1b-130">Especifica o tipo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-130">Specifies the type of the app.</span></span>  <br/> |
|<span data-ttu-id="e7f1b-131">Escopo</span><span class="sxs-lookup"><span data-stu-id="e7f1b-131">Scope</span></span>  <br/> |<span data-ttu-id="e7f1b-132">Especifica o escopo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-132">Specifies the scope of the app.</span></span>  <br/> |
|<span data-ttu-id="e7f1b-133">MarketplaceAssetId</span><span class="sxs-lookup"><span data-stu-id="e7f1b-133">MarketplaceAssetId</span></span>  <br/> |<span data-ttu-id="e7f1b-134">Especifica o identificador de ativos do Marketplace do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-134">Specifies the marketplace asset identifier of the app.</span></span>  <br/> |
|<span data-ttu-id="e7f1b-135">MarketplaceContentMarket</span><span class="sxs-lookup"><span data-stu-id="e7f1b-135">MarketplaceContentMarket</span></span>  <br/> |<span data-ttu-id="e7f1b-136">Especifica o conteúdo do Marketplace que um usuário vê para obter detalhes e revisões sobre um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-136">Specifies the marketplace content that a user sees for details and reviews about an app.</span></span>  <br/> |
|<span data-ttu-id="e7f1b-137">AppStatus</span><span class="sxs-lookup"><span data-stu-id="e7f1b-137">AppStatus</span></span>  <br/> |<span data-ttu-id="e7f1b-138">Especifica o código de status de um aplicativo de email em um estado inesperado.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-138">Specifies the status code of a mail app in an unexpected state.</span></span>  <br/> |
|<span data-ttu-id="e7f1b-139">Etoken</span><span class="sxs-lookup"><span data-stu-id="e7f1b-139">Etoken</span></span>  <br/> |<span data-ttu-id="e7f1b-140">Especifica o token de licença para aplicativos de email pagos ou de avaliação.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-140">Specifies the license token for paid or trial mail apps.</span></span>  <br/> |
   
#### <a name="type"></a><span data-ttu-id="e7f1b-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7f1b-141">Type</span></span>

|<span data-ttu-id="e7f1b-142">**Valor**</span><span class="sxs-lookup"><span data-stu-id="e7f1b-142">**Value**</span></span>|<span data-ttu-id="e7f1b-143">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e7f1b-143">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e7f1b-144">Padrão</span><span class="sxs-lookup"><span data-stu-id="e7f1b-144">Default</span></span>  <br/> |<span data-ttu-id="e7f1b-145">Indica que o aplicativo está disponível por padrão.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-145">Indicates that the app is available by default.</span></span>  <br/> |
|<span data-ttu-id="e7f1b-146">Private</span><span class="sxs-lookup"><span data-stu-id="e7f1b-146">Private</span></span>  <br/> |<span data-ttu-id="e7f1b-147">Indica que o aplicativo é privado.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-147">Indicates that the app is private.</span></span>  <br/> |
|<span data-ttu-id="e7f1b-148">Competitivo</span><span class="sxs-lookup"><span data-stu-id="e7f1b-148">MarketPlace</span></span>  <br/> |<span data-ttu-id="e7f1b-149">Indica que o aplicativo é um aplicativo de Marketplace.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-149">Indicates that the app is a marketplace app.</span></span>  <br/> |
   
#### <a name="scope"></a><span data-ttu-id="e7f1b-150">Escopo</span><span class="sxs-lookup"><span data-stu-id="e7f1b-150">Scope</span></span>

|<span data-ttu-id="e7f1b-151">**Valor**</span><span class="sxs-lookup"><span data-stu-id="e7f1b-151">**Value**</span></span>|<span data-ttu-id="e7f1b-152">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e7f1b-152">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e7f1b-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e7f1b-153">None</span></span>  <br/> |<span data-ttu-id="e7f1b-154">Indica que o aplicativo não tem escopo.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-154">Indicates that the app has no scope.</span></span>  <br/> |
|<span data-ttu-id="e7f1b-155">Usuário</span><span class="sxs-lookup"><span data-stu-id="e7f1b-155">User</span></span>  <br/> |<span data-ttu-id="e7f1b-156">Indica que o aplicativo é por usuário.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-156">Indicates that the app is per user.</span></span>  <br/> |
|<span data-ttu-id="e7f1b-157">Organização</span><span class="sxs-lookup"><span data-stu-id="e7f1b-157">Organization</span></span>  <br/> |<span data-ttu-id="e7f1b-158">Indica que o aplicativo é para uma organização.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-158">Indicates that the app is for an organization.</span></span>  <br/> |
|<span data-ttu-id="e7f1b-159">Padrão</span><span class="sxs-lookup"><span data-stu-id="e7f1b-159">Default</span></span>  <br/> |<span data-ttu-id="e7f1b-160">Indica que o aplicativo é um aplicativo padrão.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-160">Indicates that the app is a default app.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e7f1b-161">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e7f1b-161">Child elements</span></span>

|<span data-ttu-id="e7f1b-162">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e7f1b-162">**Element**</span></span>|<span data-ttu-id="e7f1b-163">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e7f1b-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7f1b-164">SpecificUsers</span><span class="sxs-lookup"><span data-stu-id="e7f1b-164">SpecificUsers</span></span>](specificusers.md) <br/> |<span data-ttu-id="e7f1b-165">Especifica as contas de email que podem acessar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-165">Specifies the email accounts that can access the app.</span></span>  <br/> |
|[<span data-ttu-id="e7f1b-166">Manifesto</span><span class="sxs-lookup"><span data-stu-id="e7f1b-166">Manifest</span></span>](manifest.md) <br/> |<span data-ttu-id="e7f1b-167">Contém o arquivo de manifesto de aplicativo codificado em base 64.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-167">Contains the base-64 encoded app manifest file.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e7f1b-168">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e7f1b-168">Parent elements</span></span>

|<span data-ttu-id="e7f1b-169">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e7f1b-169">**Element**</span></span>|<span data-ttu-id="e7f1b-170">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e7f1b-170">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7f1b-171">ClientExtensions</span><span class="sxs-lookup"><span data-stu-id="e7f1b-171">ClientExtensions</span></span>](clientextensions.md) <br/> |<span data-ttu-id="e7f1b-172">Especifica uma matriz de elementos **ClientExtension** .</span><span class="sxs-lookup"><span data-stu-id="e7f1b-172">Specifies an array of **ClientExtension** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e7f1b-173">Comentários</span><span class="sxs-lookup"><span data-stu-id="e7f1b-173">Remarks</span></span>

<span data-ttu-id="e7f1b-174">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-174">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e7f1b-175">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e7f1b-175">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7f1b-176">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e7f1b-176">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7f1b-177">Namespace</span><span class="sxs-lookup"><span data-stu-id="e7f1b-177">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e7f1b-178">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e7f1b-178">Schema Name</span></span>  <br/> |<span data-ttu-id="e7f1b-179">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="e7f1b-179">Type schema</span></span>  <br/> |
|<span data-ttu-id="e7f1b-180">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e7f1b-180">Validation File</span></span>  <br/> |<span data-ttu-id="e7f1b-181">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e7f1b-181">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e7f1b-182">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e7f1b-182">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e7f1b-183">Também consulte</span><span class="sxs-lookup"><span data-stu-id="e7f1b-183">See also</span></span>



- [<span data-ttu-id="e7f1b-184">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e7f1b-184">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

