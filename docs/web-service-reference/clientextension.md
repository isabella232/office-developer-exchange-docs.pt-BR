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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460194"
---
# <a name="clientextension"></a><span data-ttu-id="41060-103">ClientExtension</span><span class="sxs-lookup"><span data-stu-id="41060-103">ClientExtension</span></span>

<span data-ttu-id="41060-104">O elemento **ClientExtension** contém informações de usuário e configuração sobre um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="41060-104">The **ClientExtension** element contains user and configuration information about an app.</span></span> 
  
```XML
<ClientExtension IsAvailable=" true | false " IsMandatory=" true | false " IsEnabledByDefault=" true | false " Type="" Scope="" MarketplaceAssetId="" MarketplaceContentMarket="" AppStatus="" Etoken="">
    <SpecificUsers></SpecificUsers>
    <Manifest></Manifest>
</ClientExtension>
```

 <span data-ttu-id="41060-105">**ClientExtensionType**</span><span class="sxs-lookup"><span data-stu-id="41060-105">**ClientExtensionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="41060-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="41060-106">Attributes and elements</span></span>

<span data-ttu-id="41060-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="41060-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41060-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="41060-108">Attributes</span></span>

|<span data-ttu-id="41060-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="41060-109">**Attribute**</span></span>|<span data-ttu-id="41060-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41060-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="41060-111">IsAvailable</span><span class="sxs-lookup"><span data-stu-id="41060-111">IsAvailable</span></span>  <br/> |<span data-ttu-id="41060-112">Especifica se o aplicativo está disponível.</span><span class="sxs-lookup"><span data-stu-id="41060-112">Specifies whether the app is available.</span></span> <span data-ttu-id="41060-113">Um valor de texto **true** para o atributo **IsAvailable** indica que o aplicativo está disponível.</span><span class="sxs-lookup"><span data-stu-id="41060-113">A text value of **true** for the **IsAvailable** attribute indicates that the app is available.</span></span> <span data-ttu-id="41060-114">Um valor **false** indica que o aplicativo não está disponível.</span><span class="sxs-lookup"><span data-stu-id="41060-114">A value of **false** indicates that the app is not available.</span></span> <span data-ttu-id="41060-115">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="41060-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="41060-116">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="41060-116">IsMandatory</span></span>  <br/> |<span data-ttu-id="41060-117">Especifica se o aplicativo é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41060-117">Specifies whether the app is mandatory.</span></span> <span data-ttu-id="41060-118">Um valor de texto **true** para o atributo **IsMandatory** indica que o aplicativo é obrigatório para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="41060-118">A text value of **true** for the **IsMandatory** attribute indicates that the app is mandatory for the mailbox.</span></span> <span data-ttu-id="41060-119">Um valor **false** indica que o aplicativo não é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41060-119">A value of **false** indicates that the app is not mandatory.</span></span> <span data-ttu-id="41060-120">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="41060-120">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="41060-121">IsEnabledByDefault</span><span class="sxs-lookup"><span data-stu-id="41060-121">IsEnabledByDefault</span></span>  <br/> |<span data-ttu-id="41060-122">Especifica se o aplicativo está habilitado por padrão.</span><span class="sxs-lookup"><span data-stu-id="41060-122">Specifies whether the app is enabled by default.</span></span> <span data-ttu-id="41060-123">Um valor de texto **true** para o atributo **IsEnabledByDefault** indica que o aplicativo está habilitado por padrão.</span><span class="sxs-lookup"><span data-stu-id="41060-123">A text value of **true** for the **IsEnabledByDefault** attribute indicates that the app is enabled by default.</span></span> <span data-ttu-id="41060-124">Um valor **false** indica que o aplicativo não está habilitado por padrão.</span><span class="sxs-lookup"><span data-stu-id="41060-124">A value of **false** indicates that the app is not enabled by default.</span></span> <span data-ttu-id="41060-125">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="41060-125">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="41060-126">ProvidedTo</span><span class="sxs-lookup"><span data-stu-id="41060-126">ProvidedTo</span></span>  <br/> |<span data-ttu-id="41060-127">Especifica para quem o aplicativo é fornecido.</span><span class="sxs-lookup"><span data-stu-id="41060-127">Specifies to whom the app is provided.</span></span> <span data-ttu-id="41060-128">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="41060-128">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="41060-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="41060-129">Type</span></span>  <br/> |<span data-ttu-id="41060-130">Especifica o tipo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="41060-130">Specifies the type of the app.</span></span>  <br/> |
|<span data-ttu-id="41060-131">Escopo</span><span class="sxs-lookup"><span data-stu-id="41060-131">Scope</span></span>  <br/> |<span data-ttu-id="41060-132">Especifica o escopo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="41060-132">Specifies the scope of the app.</span></span>  <br/> |
|<span data-ttu-id="41060-133">MarketplaceAssetId</span><span class="sxs-lookup"><span data-stu-id="41060-133">MarketplaceAssetId</span></span>  <br/> |<span data-ttu-id="41060-134">Especifica o identificador de ativos do Marketplace do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="41060-134">Specifies the marketplace asset identifier of the app.</span></span>  <br/> |
|<span data-ttu-id="41060-135">MarketplaceContentMarket</span><span class="sxs-lookup"><span data-stu-id="41060-135">MarketplaceContentMarket</span></span>  <br/> |<span data-ttu-id="41060-136">Especifica o conteúdo do Marketplace que um usuário vê para obter detalhes e revisões sobre um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="41060-136">Specifies the marketplace content that a user sees for details and reviews about an app.</span></span>  <br/> |
|<span data-ttu-id="41060-137">AppStatus</span><span class="sxs-lookup"><span data-stu-id="41060-137">AppStatus</span></span>  <br/> |<span data-ttu-id="41060-138">Especifica o código de status de um aplicativo de email em um estado inesperado.</span><span class="sxs-lookup"><span data-stu-id="41060-138">Specifies the status code of a mail app in an unexpected state.</span></span>  <br/> |
|<span data-ttu-id="41060-139">Etoken</span><span class="sxs-lookup"><span data-stu-id="41060-139">Etoken</span></span>  <br/> |<span data-ttu-id="41060-140">Especifica o token de licença para aplicativos de email pagos ou de avaliação.</span><span class="sxs-lookup"><span data-stu-id="41060-140">Specifies the license token for paid or trial mail apps.</span></span>  <br/> |
   
#### <a name="type"></a><span data-ttu-id="41060-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="41060-141">Type</span></span>

|<span data-ttu-id="41060-142">**Valor**</span><span class="sxs-lookup"><span data-stu-id="41060-142">**Value**</span></span>|<span data-ttu-id="41060-143">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41060-143">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="41060-144">Padrão</span><span class="sxs-lookup"><span data-stu-id="41060-144">Default</span></span>  <br/> |<span data-ttu-id="41060-145">Indica que o aplicativo está disponível por padrão.</span><span class="sxs-lookup"><span data-stu-id="41060-145">Indicates that the app is available by default.</span></span>  <br/> |
|<span data-ttu-id="41060-146">Private</span><span class="sxs-lookup"><span data-stu-id="41060-146">Private</span></span>  <br/> |<span data-ttu-id="41060-147">Indica que o aplicativo é privado.</span><span class="sxs-lookup"><span data-stu-id="41060-147">Indicates that the app is private.</span></span>  <br/> |
|<span data-ttu-id="41060-148">Competitivo</span><span class="sxs-lookup"><span data-stu-id="41060-148">MarketPlace</span></span>  <br/> |<span data-ttu-id="41060-149">Indica que o aplicativo é um aplicativo de Marketplace.</span><span class="sxs-lookup"><span data-stu-id="41060-149">Indicates that the app is a marketplace app.</span></span>  <br/> |
   
#### <a name="scope"></a><span data-ttu-id="41060-150">Escopo</span><span class="sxs-lookup"><span data-stu-id="41060-150">Scope</span></span>

|<span data-ttu-id="41060-151">**Valor**</span><span class="sxs-lookup"><span data-stu-id="41060-151">**Value**</span></span>|<span data-ttu-id="41060-152">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41060-152">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="41060-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="41060-153">None</span></span>  <br/> |<span data-ttu-id="41060-154">Indica que o aplicativo não tem escopo.</span><span class="sxs-lookup"><span data-stu-id="41060-154">Indicates that the app has no scope.</span></span>  <br/> |
|<span data-ttu-id="41060-155">Usuário</span><span class="sxs-lookup"><span data-stu-id="41060-155">User</span></span>  <br/> |<span data-ttu-id="41060-156">Indica que o aplicativo é por usuário.</span><span class="sxs-lookup"><span data-stu-id="41060-156">Indicates that the app is per user.</span></span>  <br/> |
|<span data-ttu-id="41060-157">Organização</span><span class="sxs-lookup"><span data-stu-id="41060-157">Organization</span></span>  <br/> |<span data-ttu-id="41060-158">Indica que o aplicativo é para uma organização.</span><span class="sxs-lookup"><span data-stu-id="41060-158">Indicates that the app is for an organization.</span></span>  <br/> |
|<span data-ttu-id="41060-159">Padrão</span><span class="sxs-lookup"><span data-stu-id="41060-159">Default</span></span>  <br/> |<span data-ttu-id="41060-160">Indica que o aplicativo é um aplicativo padrão.</span><span class="sxs-lookup"><span data-stu-id="41060-160">Indicates that the app is a default app.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="41060-161">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="41060-161">Child elements</span></span>

|<span data-ttu-id="41060-162">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="41060-162">**Element**</span></span>|<span data-ttu-id="41060-163">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41060-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41060-164">SpecificUsers</span><span class="sxs-lookup"><span data-stu-id="41060-164">SpecificUsers</span></span>](specificusers.md) <br/> |<span data-ttu-id="41060-165">Especifica as contas de email que podem acessar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="41060-165">Specifies the email accounts that can access the app.</span></span>  <br/> |
|[<span data-ttu-id="41060-166">Manifesto</span><span class="sxs-lookup"><span data-stu-id="41060-166">Manifest</span></span>](manifest.md) <br/> |<span data-ttu-id="41060-167">Contém o arquivo de manifesto de aplicativo codificado em base 64.</span><span class="sxs-lookup"><span data-stu-id="41060-167">Contains the base-64 encoded app manifest file.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="41060-168">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="41060-168">Parent elements</span></span>

|<span data-ttu-id="41060-169">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="41060-169">**Element**</span></span>|<span data-ttu-id="41060-170">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41060-170">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41060-171">ClientExtensions</span><span class="sxs-lookup"><span data-stu-id="41060-171">ClientExtensions</span></span>](clientextensions.md) <br/> |<span data-ttu-id="41060-172">Especifica uma matriz de elementos **ClientExtension** .</span><span class="sxs-lookup"><span data-stu-id="41060-172">Specifies an array of **ClientExtension** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="41060-173">Comentários</span><span class="sxs-lookup"><span data-stu-id="41060-173">Remarks</span></span>

<span data-ttu-id="41060-174">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="41060-174">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="41060-175">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="41060-175">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="41060-176">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="41060-176">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="41060-177">Namespace</span><span class="sxs-lookup"><span data-stu-id="41060-177">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="41060-178">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="41060-178">Schema Name</span></span>  <br/> |<span data-ttu-id="41060-179">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="41060-179">Type schema</span></span>  <br/> |
|<span data-ttu-id="41060-180">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="41060-180">Validation File</span></span>  <br/> |<span data-ttu-id="41060-181">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="41060-181">types.xsd</span></span>  <br/> |
|<span data-ttu-id="41060-182">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="41060-182">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="41060-183">Confira também</span><span class="sxs-lookup"><span data-stu-id="41060-183">See also</span></span>



- [<span data-ttu-id="41060-184">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="41060-184">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

