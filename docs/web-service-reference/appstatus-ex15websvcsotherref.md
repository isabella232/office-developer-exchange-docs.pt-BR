---
title: AppStatus
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f3ab8bf1-abc5-45cf-a2e1-d7602f2c24ec
description: O valor do elemento AppStatus indica o status do aplicativo de email.
ms.openlocfilehash: d833947fd62d500418f257829d241a2e0b3bca9c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464774"
---
# <a name="appstatus"></a><span data-ttu-id="33d5d-103">AppStatus</span><span class="sxs-lookup"><span data-stu-id="33d5d-103">AppStatus</span></span>

<span data-ttu-id="33d5d-104">O valor do elemento **AppStatus** indica o status do aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="33d5d-104">The **AppStatus** element value indicates the status of the mail app.</span></span> 
  
```XML
<AppStatus/>
```

 <span data-ttu-id="33d5d-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="33d5d-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33d5d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="33d5d-106">Attributes and elements</span></span>

<span data-ttu-id="33d5d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="33d5d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33d5d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="33d5d-108">Attributes</span></span>

<span data-ttu-id="33d5d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33d5d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33d5d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="33d5d-110">Child elements</span></span>

<span data-ttu-id="33d5d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="33d5d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="33d5d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="33d5d-112">Parent elements</span></span>

[<span data-ttu-id="33d5d-113">Metadata</span><span class="sxs-lookup"><span data-stu-id="33d5d-113">Metadata</span></span>](metadata-ex15websvcsotherref.md)
  
## <a name="text-value"></a><span data-ttu-id="33d5d-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="33d5d-114">Text value</span></span>

<span data-ttu-id="33d5d-115">O valor de texto do elemento **AppStatus** indica o status do aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="33d5d-115">The text value of the **AppStatus** element indicates the status of the mail app.</span></span> <span data-ttu-id="33d5d-116">Se o usuário puder corrigir um problema relacionado ao status do aplicativo de email, o elemento [ActionUrl](actionurl.md) fornecerá a URL para executar a correção.</span><span class="sxs-lookup"><span data-stu-id="33d5d-116">If the user can fix an issue related to the status of the mail app, the [ActionUrl](actionurl.md) element provides the URL to perform the fix.</span></span> 
  
<span data-ttu-id="33d5d-117">**Tabela 1. Valores de AppStatus**</span><span class="sxs-lookup"><span data-stu-id="33d5d-117">**Table 1. AppStatus values**</span></span>

|<span data-ttu-id="33d5d-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="33d5d-118">**Value**</span></span>|<span data-ttu-id="33d5d-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="33d5d-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="33d5d-120">Nulo ou 0</span><span class="sxs-lookup"><span data-stu-id="33d5d-120">Null or 0</span></span>  <br/> |<span data-ttu-id="33d5d-121">O aplicativo de email tem um status Íntegro.</span><span class="sxs-lookup"><span data-stu-id="33d5d-121">The mail app has a healthy status.</span></span>  <br/> |
|<span data-ttu-id="33d5d-122">1.0</span><span class="sxs-lookup"><span data-stu-id="33d5d-122">1.0</span></span>  <br/> |<span data-ttu-id="33d5d-123">O aplicativo de email não pôde ser atualizado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="33d5d-123">The mail app could not be automatically updated.</span></span> <span data-ttu-id="33d5d-124">O aplicativo de email precisa ser reinstalado da Office Store.</span><span class="sxs-lookup"><span data-stu-id="33d5d-124">The mail app needs to be re-installed from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="33d5d-125">1.1</span><span class="sxs-lookup"><span data-stu-id="33d5d-125">1.1</span></span>  <br/> |<span data-ttu-id="33d5d-126">O aplicativo de email não pôde ser atualizado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="33d5d-126">The mail app could not be automatically updated.</span></span> <span data-ttu-id="33d5d-127">O aplicativo de email requer mais permissões, e isso exige que a revisão e a confirmação sejam instaladas.</span><span class="sxs-lookup"><span data-stu-id="33d5d-127">The mail app requires increased permissions, and this requires your review and confirmation to install.</span></span>  <br/> |
|<span data-ttu-id="33d5d-128">1.2</span><span class="sxs-lookup"><span data-stu-id="33d5d-128">1.2</span></span>  <br/> |<span data-ttu-id="33d5d-129">O aplicativo de email não pôde ser atualizado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="33d5d-129">The mail app couldn't be updated automatically.</span></span> <span data-ttu-id="33d5d-130">A licença atual expirou ou é inválida.</span><span class="sxs-lookup"><span data-stu-id="33d5d-130">The current license has expired or is invalid.</span></span> <span data-ttu-id="33d5d-131">Atualize o aplicativo de email da Office Store.</span><span class="sxs-lookup"><span data-stu-id="33d5d-131">Please update the mail app from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="33d5d-132">2.0</span><span class="sxs-lookup"><span data-stu-id="33d5d-132">2.0</span></span>  <br/> |<span data-ttu-id="33d5d-133">A licença do aplicativo de email não pôde ser atualizada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="33d5d-133">The mail app license could not be automatically updated.</span></span> <span data-ttu-id="33d5d-134">A licença do aplicativo de email precisa ser recuperada da Office Store.</span><span class="sxs-lookup"><span data-stu-id="33d5d-134">The license for the mail app needs to be recovered from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="33d5d-135">2.1</span><span class="sxs-lookup"><span data-stu-id="33d5d-135">2.1</span></span>  <br/> |<span data-ttu-id="33d5d-136">A licença do aplicativo de email não pôde ser atualizada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="33d5d-136">The mail app license could not be automatically updated.</span></span> <span data-ttu-id="33d5d-137">A licença atual expirou.</span><span class="sxs-lookup"><span data-stu-id="33d5d-137">The current license has expired.</span></span> <span data-ttu-id="33d5d-138">Uma nova licença para este aplicativo precisa ser instalada da Office Store.</span><span class="sxs-lookup"><span data-stu-id="33d5d-138">A new license for this app needs to be installed from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="33d5d-139">3,0</span><span class="sxs-lookup"><span data-stu-id="33d5d-139">3.0</span></span>  <br/> |<span data-ttu-id="33d5d-140">O status da Office Store para o aplicativo de email foi alterado.</span><span class="sxs-lookup"><span data-stu-id="33d5d-140">The Office Store status for the mail app has changed.</span></span> <span data-ttu-id="33d5d-141">Isso pode indicar que há um problema com o aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="33d5d-141">This may indicate that there is a problem with the mail app.</span></span> <span data-ttu-id="33d5d-142">Vá para a página aplicativo de email na Office Store para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="33d5d-142">Go to the mail app page in the Office Store for more information.</span></span>  <br/> |
|<span data-ttu-id="33d5d-143">3.1</span><span class="sxs-lookup"><span data-stu-id="33d5d-143">3.1</span></span>  <br/> |<span data-ttu-id="33d5d-144">O aplicativo de email foi removido da Office Store.</span><span class="sxs-lookup"><span data-stu-id="33d5d-144">The mail app has been removed from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="33d5d-145">3.2</span><span class="sxs-lookup"><span data-stu-id="33d5d-145">3.2</span></span>  <br/> |<span data-ttu-id="33d5d-146">Foi descoberto um problema com o aplicativo de email e foi temporariamente retirado da Office Store.</span><span class="sxs-lookup"><span data-stu-id="33d5d-146">A problem has been discovered with the mail app and it has temporarily been withdrawn from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="33d5d-147">3.3</span><span class="sxs-lookup"><span data-stu-id="33d5d-147">3.3</span></span>  <br/> |<span data-ttu-id="33d5d-148">O aplicativo de email será removido da Office Store dentro de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="33d5d-148">The mail app will be removed from the Office Store within 30 days.</span></span>  <br/> |
|<span data-ttu-id="33d5d-149">4,0</span><span class="sxs-lookup"><span data-stu-id="33d5d-149">4.0</span></span>  <br/> |<span data-ttu-id="33d5d-150">O aplicativo de email foi desabilitado automaticamente pelo cliente de email.</span><span class="sxs-lookup"><span data-stu-id="33d5d-150">The mail app has been automatically disabled by your mail client.</span></span>  <br/> |
|<span data-ttu-id="33d5d-151">4.1</span><span class="sxs-lookup"><span data-stu-id="33d5d-151">4.1</span></span>  <br/> |<span data-ttu-id="33d5d-152">O aplicativo de email foi desabilitado pelo Outlook por motivos de desempenho.</span><span class="sxs-lookup"><span data-stu-id="33d5d-152">The mail app has been disabled by Outlook for performance reasons.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="33d5d-153">Comentários</span><span class="sxs-lookup"><span data-stu-id="33d5d-153">Remarks</span></span>

<span data-ttu-id="33d5d-154">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="33d5d-154">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="33d5d-155">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="33d5d-155">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="33d5d-156">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="33d5d-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33d5d-157">Namespace</span><span class="sxs-lookup"><span data-stu-id="33d5d-157">Namespace</span></span>  <br/> | https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="33d5d-158">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="33d5d-158">Schema Name</span></span>  <br/> |<span data-ttu-id="33d5d-159">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="33d5d-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="33d5d-160">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="33d5d-160">Validation File</span></span>  <br/> |<span data-ttu-id="33d5d-161">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="33d5d-161">Not applicable</span></span>  <br/> |
|<span data-ttu-id="33d5d-162">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="33d5d-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="33d5d-163">False</span><span class="sxs-lookup"><span data-stu-id="33d5d-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="33d5d-164">Confira também</span><span class="sxs-lookup"><span data-stu-id="33d5d-164">See also</span></span>

- [<span data-ttu-id="33d5d-165">Metadata</span><span class="sxs-lookup"><span data-stu-id="33d5d-165">Metadata</span></span>](metadata-ex15websvcsotherref.md)
- [<span data-ttu-id="33d5d-166">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="33d5d-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

