---
title: FieldUri (regra)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cecdea78-de9c-48be-ae31-03877feafeec
description: O elemento FieldURI especifica o URI para o campo de regra que causou o erro de validação.
ms.openlocfilehash: 3d88efdf951af580f81b5e2e7a544dcdf70ea830
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461244"
---
# <a name="fielduri-rule"></a><span data-ttu-id="72a77-103">FieldUri (regra)</span><span class="sxs-lookup"><span data-stu-id="72a77-103">FieldUri (Rule)</span></span>

<span data-ttu-id="72a77-104">O elemento **FieldURI** especifica o URI para o campo de regra que causou o erro de validação.</span><span class="sxs-lookup"><span data-stu-id="72a77-104">The **FieldURI** element specifies the URI to the rule field that caused the validation error.</span></span> 
  
```XML
<FieldURI/>
```

 <span data-ttu-id="72a77-105">**RuleFieldURIType**</span><span class="sxs-lookup"><span data-stu-id="72a77-105">**RuleFieldURIType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="72a77-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="72a77-106">Attributes and elements</span></span>

<span data-ttu-id="72a77-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="72a77-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="72a77-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="72a77-108">Attributes</span></span>

<span data-ttu-id="72a77-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="72a77-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="72a77-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="72a77-110">Child elements</span></span>

<span data-ttu-id="72a77-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="72a77-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="72a77-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="72a77-112">Parent elements</span></span>

|<span data-ttu-id="72a77-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="72a77-113">**Element**</span></span>|<span data-ttu-id="72a77-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="72a77-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72a77-115">Erro</span><span class="sxs-lookup"><span data-stu-id="72a77-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="72a77-116">Representa um único erro de validação em um valor de propriedade de regra específico, um valor da propriedade Predicate ou um valor da propriedade Action.</span><span class="sxs-lookup"><span data-stu-id="72a77-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="72a77-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="72a77-117">Text value</span></span>

<span data-ttu-id="72a77-118">O valor de texto para este elemento é restrito a uma das seguintes cadeias de caracteres:</span><span class="sxs-lookup"><span data-stu-id="72a77-118">The text value for this element is restricted to one of the following strings:</span></span>
  
- <span data-ttu-id="72a77-119">RuleId</span><span class="sxs-lookup"><span data-stu-id="72a77-119">RuleId</span></span>
    
- <span data-ttu-id="72a77-120">DisplayName</span><span class="sxs-lookup"><span data-stu-id="72a77-120">DisplayName</span></span>
    
- <span data-ttu-id="72a77-121">Prioridade</span><span class="sxs-lookup"><span data-stu-id="72a77-121">Priority</span></span>
    
- <span data-ttu-id="72a77-122">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="72a77-122">IsNotSupported</span></span>
    
- <span data-ttu-id="72a77-123">Ações</span><span class="sxs-lookup"><span data-stu-id="72a77-123">Actions</span></span>
    
- <span data-ttu-id="72a77-124">Condição: categorias</span><span class="sxs-lookup"><span data-stu-id="72a77-124">Condition:Categories</span></span>
    
- <span data-ttu-id="72a77-125">Condição: ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="72a77-125">Condition:ContainsBodyStrings</span></span>
    
- <span data-ttu-id="72a77-126">Condição: ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="72a77-126">Condition:ContainsHeaderStrings</span></span>
    
- <span data-ttu-id="72a77-127">Condição: ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="72a77-127">Condition:ContainsRecipientStrings</span></span>
    
- <span data-ttu-id="72a77-128">Condição: ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="72a77-128">Condition:ContainsSenderStrings</span></span>
    
- <span data-ttu-id="72a77-129">Condição: ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="72a77-129">Condition:ContainsSubjectOrBodyStrings</span></span>
    
- <span data-ttu-id="72a77-130">Condição: ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="72a77-130">Condition:ContainsSubjectStrings</span></span>
    
- <span data-ttu-id="72a77-131">Condição: FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="72a77-131">Condition:FlaggedForAction</span></span>
    
- <span data-ttu-id="72a77-132">Condição: FromAddresses</span><span class="sxs-lookup"><span data-stu-id="72a77-132">Condition:FromAddresses</span></span>
    
- <span data-ttu-id="72a77-133">Condição: FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="72a77-133">Condition:FromConnectedAccounts</span></span>
    
- <span data-ttu-id="72a77-134">Condição: HasAttachments</span><span class="sxs-lookup"><span data-stu-id="72a77-134">Condition:HasAttachments</span></span>
    
- <span data-ttu-id="72a77-135">Condição: importância</span><span class="sxs-lookup"><span data-stu-id="72a77-135">Condition:Importance</span></span>
    
- <span data-ttu-id="72a77-136">Condição: IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="72a77-136">Condition:IsApprovalRequest</span></span>
    
- <span data-ttu-id="72a77-137">Condição: IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="72a77-137">Condition:IsAutomaticForward</span></span>
    
- <span data-ttu-id="72a77-138">Condição: IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="72a77-138">Condition:IsAutomaticReply</span></span>
    
- <span data-ttu-id="72a77-139">Condição: IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="72a77-139">Condition:IsEncrypted</span></span>
    
- <span data-ttu-id="72a77-140">Condição: IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="72a77-140">Condition:IsMeetingRequest</span></span>
    
- <span data-ttu-id="72a77-141">Condição: IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="72a77-141">Condition:IsMeetingResponse</span></span>
    
- <span data-ttu-id="72a77-142">Condição: IsNDR</span><span class="sxs-lookup"><span data-stu-id="72a77-142">Condition:IsNDR</span></span>
    
- <span data-ttu-id="72a77-143">Condição: IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="72a77-143">Condition:IsPermissionControlled</span></span>
    
- <span data-ttu-id="72a77-144">Condição: IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="72a77-144">Condition:IsReadReceipt</span></span>
    
- <span data-ttu-id="72a77-145">Condição: IsSigned</span><span class="sxs-lookup"><span data-stu-id="72a77-145">Condition:IsSigned</span></span>
    
- <span data-ttu-id="72a77-146">Condição: iscaixa postal</span><span class="sxs-lookup"><span data-stu-id="72a77-146">Condition:IsVoicemail</span></span>
    
- <span data-ttu-id="72a77-147">Condição: doclasss</span><span class="sxs-lookup"><span data-stu-id="72a77-147">Condition:ItemClasses</span></span>
    
- <span data-ttu-id="72a77-148">Condição: MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="72a77-148">Condition:MessageClassifications</span></span>
    
- <span data-ttu-id="72a77-149">Condição: NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="72a77-149">Condition:NotSentToMe</span></span>
    
- <span data-ttu-id="72a77-150">Condição: SentCcMe</span><span class="sxs-lookup"><span data-stu-id="72a77-150">Condition:SentCcMe</span></span>
    
- <span data-ttu-id="72a77-151">Condição: SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="72a77-151">Condition:SentOnlyToMe</span></span>
    
- <span data-ttu-id="72a77-152">Condição: SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="72a77-152">Condition:SentToAddresses</span></span>
    
- <span data-ttu-id="72a77-153">Condição: SentToMe</span><span class="sxs-lookup"><span data-stu-id="72a77-153">Condition:SentToMe</span></span>
    
- <span data-ttu-id="72a77-154">Condição: SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="72a77-154">Condition:SentToOrCcMe</span></span>
    
- <span data-ttu-id="72a77-155">Condição: sensibilidade</span><span class="sxs-lookup"><span data-stu-id="72a77-155">Condition:Sensitivity</span></span>
    
- <span data-ttu-id="72a77-156">Condição: WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="72a77-156">Condition:WithinDateRange</span></span>
    
- <span data-ttu-id="72a77-157">Condição: WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="72a77-157">Condition:WithinSizeRange</span></span>
    
- <span data-ttu-id="72a77-158">Exceção: categorias</span><span class="sxs-lookup"><span data-stu-id="72a77-158">Exception:Categories</span></span>
    
- <span data-ttu-id="72a77-159">Exceção: ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="72a77-159">Exception:ContainsBodyStrings</span></span>
    
- <span data-ttu-id="72a77-160">Exceção: ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="72a77-160">Exception:ContainsHeaderStrings</span></span>
    
- <span data-ttu-id="72a77-161">Exceção: ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="72a77-161">Exception:ContainsRecipientStrings</span></span>
    
- <span data-ttu-id="72a77-162">Exceção: ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="72a77-162">Exception:ContainsSenderStrings</span></span>
    
- <span data-ttu-id="72a77-163">Exceção: ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="72a77-163">Exception:ContainsSubjectOrBodyStrings</span></span>
    
- <span data-ttu-id="72a77-164">Exceção: ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="72a77-164">Exception:ContainsSubjectStrings</span></span>
    
- <span data-ttu-id="72a77-165">Exceção: FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="72a77-165">Exception:FlaggedForAction</span></span>
    
- <span data-ttu-id="72a77-166">Exceção: FromAddresses</span><span class="sxs-lookup"><span data-stu-id="72a77-166">Exception:FromAddresses</span></span>
    
- <span data-ttu-id="72a77-167">Exceção: FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="72a77-167">Exception:FromConnectedAccounts</span></span>
    
- <span data-ttu-id="72a77-168">Exceção: HasAttachments</span><span class="sxs-lookup"><span data-stu-id="72a77-168">Exception:HasAttachments</span></span>
    
- <span data-ttu-id="72a77-169">Exceção: importância</span><span class="sxs-lookup"><span data-stu-id="72a77-169">Exception:Importance</span></span>
    
- <span data-ttu-id="72a77-170">Exceção: IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="72a77-170">Exception:IsApprovalRequest</span></span>
    
- <span data-ttu-id="72a77-171">Exceção: IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="72a77-171">Exception:IsAutomaticForward</span></span>
    
- <span data-ttu-id="72a77-172">Exceção: IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="72a77-172">Exception:IsAutomaticReply</span></span>
    
- <span data-ttu-id="72a77-173">Exceção: IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="72a77-173">Exception:IsEncrypted</span></span>
    
- <span data-ttu-id="72a77-174">Exceção: IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="72a77-174">Exception:IsMeetingRequest</span></span>
    
- <span data-ttu-id="72a77-175">Exceção: IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="72a77-175">Exception:IsMeetingResponse</span></span>
    
- <span data-ttu-id="72a77-176">Exceção: IsNDR</span><span class="sxs-lookup"><span data-stu-id="72a77-176">Exception:IsNDR</span></span>
    
- <span data-ttu-id="72a77-177">Exceção: IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="72a77-177">Exception:IsPermissionControlled</span></span>
    
- <span data-ttu-id="72a77-178">Exceção: IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="72a77-178">Exception:IsReadReceipt</span></span>
    
- <span data-ttu-id="72a77-179">Exceção: IsSigned</span><span class="sxs-lookup"><span data-stu-id="72a77-179">Exception:IsSigned</span></span>
    
- <span data-ttu-id="72a77-180">Exceção: ispostal</span><span class="sxs-lookup"><span data-stu-id="72a77-180">Exception:IsVoicemail</span></span>
    
- <span data-ttu-id="72a77-181">Exceção: doclasss</span><span class="sxs-lookup"><span data-stu-id="72a77-181">Exception:ItemClasses</span></span>
    
- <span data-ttu-id="72a77-182">Exceção: MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="72a77-182">Exception:MessageClassifications</span></span>
    
- <span data-ttu-id="72a77-183">Exceção: NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="72a77-183">Exception:NotSentToMe</span></span>
    
- <span data-ttu-id="72a77-184">Exceção: SentCcMe</span><span class="sxs-lookup"><span data-stu-id="72a77-184">Exception:SentCcMe</span></span>
    
- <span data-ttu-id="72a77-185">Exceção: SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="72a77-185">Exception:SentOnlyToMe</span></span>
    
- <span data-ttu-id="72a77-186">Exceção: SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="72a77-186">Exception:SentToAddresses</span></span>
    
- <span data-ttu-id="72a77-187">Exceção: SentToMe</span><span class="sxs-lookup"><span data-stu-id="72a77-187">Exception:SentToMe</span></span>
    
- <span data-ttu-id="72a77-188">Exceção: SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="72a77-188">Exception:SentToOrCcMe</span></span>
    
- <span data-ttu-id="72a77-189">Exceção: sensibilidade</span><span class="sxs-lookup"><span data-stu-id="72a77-189">Exception:Sensitivity</span></span>
    
- <span data-ttu-id="72a77-190">Exceção: WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="72a77-190">Exception:WithinDateRange</span></span>
    
- <span data-ttu-id="72a77-191">Exceção: WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="72a77-191">Exception:WithinSizeRange</span></span>
    
- <span data-ttu-id="72a77-192">Ação: AssignCategories</span><span class="sxs-lookup"><span data-stu-id="72a77-192">Action:AssignCategories</span></span>
    
- <span data-ttu-id="72a77-193">Ação: CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="72a77-193">Action:CopyToFolder</span></span>
    
- <span data-ttu-id="72a77-194">Ação: excluir</span><span class="sxs-lookup"><span data-stu-id="72a77-194">Action:Delete</span></span>
    
- <span data-ttu-id="72a77-195">Ação: ForwardAsAttachmentToRecipients</span><span class="sxs-lookup"><span data-stu-id="72a77-195">Action:ForwardAsAttachmentToRecipients</span></span>
    
- <span data-ttu-id="72a77-196">Ação: ForwardToRecipients</span><span class="sxs-lookup"><span data-stu-id="72a77-196">Action:ForwardToRecipients</span></span>
    
- <span data-ttu-id="72a77-197">Ação: MarkImportance</span><span class="sxs-lookup"><span data-stu-id="72a77-197">Action:MarkImportance</span></span>
    
- <span data-ttu-id="72a77-198">Ação: MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="72a77-198">Action:MarkAsRead</span></span>
    
- <span data-ttu-id="72a77-199">Ação: MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="72a77-199">Action:MoveToFolder</span></span>
    
- <span data-ttu-id="72a77-200">Ação: PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="72a77-200">Action:PermanentDelete</span></span>
    
- <span data-ttu-id="72a77-201">Ação: RedirectToRecipients</span><span class="sxs-lookup"><span data-stu-id="72a77-201">Action:RedirectToRecipients</span></span>
    
- <span data-ttu-id="72a77-202">Ação: SendSMSAlertToRecipients</span><span class="sxs-lookup"><span data-stu-id="72a77-202">Action:SendSMSAlertToRecipients</span></span>
    
- <span data-ttu-id="72a77-203">Ação: ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="72a77-203">Action:ServerReplyWithMessage</span></span>
    
- <span data-ttu-id="72a77-204">Ação: StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="72a77-204">Action:StopProcessingRules</span></span>
    
- <span data-ttu-id="72a77-205">IsEnabled</span><span class="sxs-lookup"><span data-stu-id="72a77-205">IsEnabled</span></span>
    
- <span data-ttu-id="72a77-206">IsInError</span><span class="sxs-lookup"><span data-stu-id="72a77-206">IsInError</span></span>
    
- <span data-ttu-id="72a77-207">Condições</span><span class="sxs-lookup"><span data-stu-id="72a77-207">Conditions</span></span>
    
- <span data-ttu-id="72a77-208">Exceções</span><span class="sxs-lookup"><span data-stu-id="72a77-208">Exceptions</span></span>
    
## <a name="remarks"></a><span data-ttu-id="72a77-209">Comentários</span><span class="sxs-lookup"><span data-stu-id="72a77-209">Remarks</span></span>

<span data-ttu-id="72a77-210">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="72a77-210">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="72a77-211">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="72a77-211">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="72a77-212">Namespace</span><span class="sxs-lookup"><span data-stu-id="72a77-212">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="72a77-213">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="72a77-213">Schema Name</span></span>  <br/> |<span data-ttu-id="72a77-214">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="72a77-214">Messages schema</span></span>  <br/> |
|<span data-ttu-id="72a77-215">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="72a77-215">Validation File</span></span>  <br/> |<span data-ttu-id="72a77-216">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="72a77-216">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="72a77-217">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="72a77-217">Can be Empty</span></span>  <br/> |<span data-ttu-id="72a77-218">False</span><span class="sxs-lookup"><span data-stu-id="72a77-218">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="72a77-219">Confira também</span><span class="sxs-lookup"><span data-stu-id="72a77-219">See also</span></span>



- [<span data-ttu-id="72a77-220">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="72a77-220">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

