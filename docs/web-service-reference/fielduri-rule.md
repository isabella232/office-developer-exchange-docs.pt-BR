---
title: FieldUri (regra)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cecdea78-de9c-48be-ae31-03877feafeec
description: O elemento FieldURI Especifica o URI para o campo de regra que causou o erro de validação.
ms.openlocfilehash: 88ba54994625d3a950b58e900f28c986c31eddac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752237"
---
# <a name="fielduri-rule"></a><span data-ttu-id="b0d71-103">FieldUri (regra)</span><span class="sxs-lookup"><span data-stu-id="b0d71-103">FieldUri (Rule)</span></span>

<span data-ttu-id="b0d71-104">O elemento **FieldURI** Especifica o URI para o campo de regra que causou o erro de validação.</span><span class="sxs-lookup"><span data-stu-id="b0d71-104">The **FieldURI** element specifies the URI to the rule field that caused the validation error.</span></span> 
  
```XML
<FieldURI/>
```

 <span data-ttu-id="b0d71-105">**RuleFieldURIType**</span><span class="sxs-lookup"><span data-stu-id="b0d71-105">**RuleFieldURIType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0d71-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b0d71-106">Attributes and elements</span></span>

<span data-ttu-id="b0d71-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b0d71-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0d71-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b0d71-108">Attributes</span></span>

<span data-ttu-id="b0d71-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b0d71-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0d71-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b0d71-110">Child elements</span></span>

<span data-ttu-id="b0d71-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b0d71-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b0d71-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b0d71-112">Parent elements</span></span>

|<span data-ttu-id="b0d71-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b0d71-113">**Element**</span></span>|<span data-ttu-id="b0d71-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b0d71-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0d71-115">Erro</span><span class="sxs-lookup"><span data-stu-id="b0d71-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="b0d71-116">Representa um erro de validação exclusivo em um valor da propriedade regra específica, o valor da propriedade predicado ou o valor da propriedade action.</span><span class="sxs-lookup"><span data-stu-id="b0d71-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b0d71-117">Text value</span><span class="sxs-lookup"><span data-stu-id="b0d71-117">Text value</span></span>

<span data-ttu-id="b0d71-118">O valor de texto para esse elemento é restrito a uma das cadeias de caracteres seguintes:</span><span class="sxs-lookup"><span data-stu-id="b0d71-118">The text value for this element is restricted to one of the following strings:</span></span>
  
- <span data-ttu-id="b0d71-119">RuleId</span><span class="sxs-lookup"><span data-stu-id="b0d71-119">RuleId</span></span>
    
- <span data-ttu-id="b0d71-120">DisplayName</span><span class="sxs-lookup"><span data-stu-id="b0d71-120">DisplayName</span></span>
    
- <span data-ttu-id="b0d71-121">Prioridade</span><span class="sxs-lookup"><span data-stu-id="b0d71-121">Priority</span></span>
    
- <span data-ttu-id="b0d71-122">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="b0d71-122">IsNotSupported</span></span>
    
- <span data-ttu-id="b0d71-123">Ações</span><span class="sxs-lookup"><span data-stu-id="b0d71-123">Actions</span></span>
    
- <span data-ttu-id="b0d71-124">Condição: categorias</span><span class="sxs-lookup"><span data-stu-id="b0d71-124">Condition:Categories</span></span>
    
- <span data-ttu-id="b0d71-125">Condição: ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="b0d71-125">Condition:ContainsBodyStrings</span></span>
    
- <span data-ttu-id="b0d71-126">Condição: ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="b0d71-126">Condition:ContainsHeaderStrings</span></span>
    
- <span data-ttu-id="b0d71-127">Condição: ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="b0d71-127">Condition:ContainsRecipientStrings</span></span>
    
- <span data-ttu-id="b0d71-128">Condição: ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="b0d71-128">Condition:ContainsSenderStrings</span></span>
    
- <span data-ttu-id="b0d71-129">Condição: ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="b0d71-129">Condition:ContainsSubjectOrBodyStrings</span></span>
    
- <span data-ttu-id="b0d71-130">Condição: ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="b0d71-130">Condition:ContainsSubjectStrings</span></span>
    
- <span data-ttu-id="b0d71-131">Condição: FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="b0d71-131">Condition:FlaggedForAction</span></span>
    
- <span data-ttu-id="b0d71-132">Condição: FromAddresses</span><span class="sxs-lookup"><span data-stu-id="b0d71-132">Condition:FromAddresses</span></span>
    
- <span data-ttu-id="b0d71-133">Condição: FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="b0d71-133">Condition:FromConnectedAccounts</span></span>
    
- <span data-ttu-id="b0d71-134">Condição: HasAttachments</span><span class="sxs-lookup"><span data-stu-id="b0d71-134">Condition:HasAttachments</span></span>
    
- <span data-ttu-id="b0d71-135">Condição: importância</span><span class="sxs-lookup"><span data-stu-id="b0d71-135">Condition:Importance</span></span>
    
- <span data-ttu-id="b0d71-136">Condição: IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="b0d71-136">Condition:IsApprovalRequest</span></span>
    
- <span data-ttu-id="b0d71-137">Condição: IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="b0d71-137">Condition:IsAutomaticForward</span></span>
    
- <span data-ttu-id="b0d71-138">Condição: IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="b0d71-138">Condition:IsAutomaticReply</span></span>
    
- <span data-ttu-id="b0d71-139">Condição: IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="b0d71-139">Condition:IsEncrypted</span></span>
    
- <span data-ttu-id="b0d71-140">Condição: IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b0d71-140">Condition:IsMeetingRequest</span></span>
    
- <span data-ttu-id="b0d71-141">Condição: IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="b0d71-141">Condition:IsMeetingResponse</span></span>
    
- <span data-ttu-id="b0d71-142">Condição: IsNDR</span><span class="sxs-lookup"><span data-stu-id="b0d71-142">Condition:IsNDR</span></span>
    
- <span data-ttu-id="b0d71-143">Condição: IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="b0d71-143">Condition:IsPermissionControlled</span></span>
    
- <span data-ttu-id="b0d71-144">Condição: IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="b0d71-144">Condition:IsReadReceipt</span></span>
    
- <span data-ttu-id="b0d71-145">Condição: IsSigned</span><span class="sxs-lookup"><span data-stu-id="b0d71-145">Condition:IsSigned</span></span>
    
- <span data-ttu-id="b0d71-146">Condição: IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="b0d71-146">Condition:IsVoicemail</span></span>
    
- <span data-ttu-id="b0d71-147">Condição: ItemClasses</span><span class="sxs-lookup"><span data-stu-id="b0d71-147">Condition:ItemClasses</span></span>
    
- <span data-ttu-id="b0d71-148">Condição: MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="b0d71-148">Condition:MessageClassifications</span></span>
    
- <span data-ttu-id="b0d71-149">Condição: NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="b0d71-149">Condition:NotSentToMe</span></span>
    
- <span data-ttu-id="b0d71-150">Condição: SentCcMe</span><span class="sxs-lookup"><span data-stu-id="b0d71-150">Condition:SentCcMe</span></span>
    
- <span data-ttu-id="b0d71-151">Condição: SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="b0d71-151">Condition:SentOnlyToMe</span></span>
    
- <span data-ttu-id="b0d71-152">Condição: SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="b0d71-152">Condition:SentToAddresses</span></span>
    
- <span data-ttu-id="b0d71-153">Condição: SentToMe</span><span class="sxs-lookup"><span data-stu-id="b0d71-153">Condition:SentToMe</span></span>
    
- <span data-ttu-id="b0d71-154">Condição: SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="b0d71-154">Condition:SentToOrCcMe</span></span>
    
- <span data-ttu-id="b0d71-155">Condição: sensibilidade</span><span class="sxs-lookup"><span data-stu-id="b0d71-155">Condition:Sensitivity</span></span>
    
- <span data-ttu-id="b0d71-156">Condição: WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="b0d71-156">Condition:WithinDateRange</span></span>
    
- <span data-ttu-id="b0d71-157">Condição: WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="b0d71-157">Condition:WithinSizeRange</span></span>
    
- <span data-ttu-id="b0d71-158">Exceção: categorias</span><span class="sxs-lookup"><span data-stu-id="b0d71-158">Exception:Categories</span></span>
    
- <span data-ttu-id="b0d71-159">Exceção: ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="b0d71-159">Exception:ContainsBodyStrings</span></span>
    
- <span data-ttu-id="b0d71-160">Exceção: ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="b0d71-160">Exception:ContainsHeaderStrings</span></span>
    
- <span data-ttu-id="b0d71-161">Exceção: ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="b0d71-161">Exception:ContainsRecipientStrings</span></span>
    
- <span data-ttu-id="b0d71-162">Exceção: ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="b0d71-162">Exception:ContainsSenderStrings</span></span>
    
- <span data-ttu-id="b0d71-163">Exceção: ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="b0d71-163">Exception:ContainsSubjectOrBodyStrings</span></span>
    
- <span data-ttu-id="b0d71-164">Exceção: ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="b0d71-164">Exception:ContainsSubjectStrings</span></span>
    
- <span data-ttu-id="b0d71-165">Exceção: FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="b0d71-165">Exception:FlaggedForAction</span></span>
    
- <span data-ttu-id="b0d71-166">Exceção: FromAddresses</span><span class="sxs-lookup"><span data-stu-id="b0d71-166">Exception:FromAddresses</span></span>
    
- <span data-ttu-id="b0d71-167">Exceção: FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="b0d71-167">Exception:FromConnectedAccounts</span></span>
    
- <span data-ttu-id="b0d71-168">Exceção: HasAttachments</span><span class="sxs-lookup"><span data-stu-id="b0d71-168">Exception:HasAttachments</span></span>
    
- <span data-ttu-id="b0d71-169">Exceção: importância</span><span class="sxs-lookup"><span data-stu-id="b0d71-169">Exception:Importance</span></span>
    
- <span data-ttu-id="b0d71-170">Exceção: IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="b0d71-170">Exception:IsApprovalRequest</span></span>
    
- <span data-ttu-id="b0d71-171">Exceção: IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="b0d71-171">Exception:IsAutomaticForward</span></span>
    
- <span data-ttu-id="b0d71-172">Exceção: IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="b0d71-172">Exception:IsAutomaticReply</span></span>
    
- <span data-ttu-id="b0d71-173">Exceção: IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="b0d71-173">Exception:IsEncrypted</span></span>
    
- <span data-ttu-id="b0d71-174">Exceção: IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b0d71-174">Exception:IsMeetingRequest</span></span>
    
- <span data-ttu-id="b0d71-175">Exceção: IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="b0d71-175">Exception:IsMeetingResponse</span></span>
    
- <span data-ttu-id="b0d71-176">Exceção: IsNDR</span><span class="sxs-lookup"><span data-stu-id="b0d71-176">Exception:IsNDR</span></span>
    
- <span data-ttu-id="b0d71-177">Exceção: IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="b0d71-177">Exception:IsPermissionControlled</span></span>
    
- <span data-ttu-id="b0d71-178">Exceção: IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="b0d71-178">Exception:IsReadReceipt</span></span>
    
- <span data-ttu-id="b0d71-179">Exceção: IsSigned</span><span class="sxs-lookup"><span data-stu-id="b0d71-179">Exception:IsSigned</span></span>
    
- <span data-ttu-id="b0d71-180">Exceção: IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="b0d71-180">Exception:IsVoicemail</span></span>
    
- <span data-ttu-id="b0d71-181">Exceção: ItemClasses</span><span class="sxs-lookup"><span data-stu-id="b0d71-181">Exception:ItemClasses</span></span>
    
- <span data-ttu-id="b0d71-182">Exceção: MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="b0d71-182">Exception:MessageClassifications</span></span>
    
- <span data-ttu-id="b0d71-183">Exceção: NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="b0d71-183">Exception:NotSentToMe</span></span>
    
- <span data-ttu-id="b0d71-184">Exceção: SentCcMe</span><span class="sxs-lookup"><span data-stu-id="b0d71-184">Exception:SentCcMe</span></span>
    
- <span data-ttu-id="b0d71-185">Exceção: SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="b0d71-185">Exception:SentOnlyToMe</span></span>
    
- <span data-ttu-id="b0d71-186">Exceção: SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="b0d71-186">Exception:SentToAddresses</span></span>
    
- <span data-ttu-id="b0d71-187">Exceção: SentToMe</span><span class="sxs-lookup"><span data-stu-id="b0d71-187">Exception:SentToMe</span></span>
    
- <span data-ttu-id="b0d71-188">Exceção: SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="b0d71-188">Exception:SentToOrCcMe</span></span>
    
- <span data-ttu-id="b0d71-189">Exceção: sensibilidade</span><span class="sxs-lookup"><span data-stu-id="b0d71-189">Exception:Sensitivity</span></span>
    
- <span data-ttu-id="b0d71-190">Exceção: WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="b0d71-190">Exception:WithinDateRange</span></span>
    
- <span data-ttu-id="b0d71-191">Exceção: WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="b0d71-191">Exception:WithinSizeRange</span></span>
    
- <span data-ttu-id="b0d71-192">Ação: AssignCategories</span><span class="sxs-lookup"><span data-stu-id="b0d71-192">Action:AssignCategories</span></span>
    
- <span data-ttu-id="b0d71-193">Ação: CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="b0d71-193">Action:CopyToFolder</span></span>
    
- <span data-ttu-id="b0d71-194">Ação: excluir</span><span class="sxs-lookup"><span data-stu-id="b0d71-194">Action:Delete</span></span>
    
- <span data-ttu-id="b0d71-195">Ação: ForwardAsAttachmentToRecipients</span><span class="sxs-lookup"><span data-stu-id="b0d71-195">Action:ForwardAsAttachmentToRecipients</span></span>
    
- <span data-ttu-id="b0d71-196">Ação: ForwardToRecipients</span><span class="sxs-lookup"><span data-stu-id="b0d71-196">Action:ForwardToRecipients</span></span>
    
- <span data-ttu-id="b0d71-197">Ação: MarkImportance</span><span class="sxs-lookup"><span data-stu-id="b0d71-197">Action:MarkImportance</span></span>
    
- <span data-ttu-id="b0d71-198">Ação: MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="b0d71-198">Action:MarkAsRead</span></span>
    
- <span data-ttu-id="b0d71-199">Ação: MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="b0d71-199">Action:MoveToFolder</span></span>
    
- <span data-ttu-id="b0d71-200">Ação: PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="b0d71-200">Action:PermanentDelete</span></span>
    
- <span data-ttu-id="b0d71-201">Ação: RedirectToRecipients</span><span class="sxs-lookup"><span data-stu-id="b0d71-201">Action:RedirectToRecipients</span></span>
    
- <span data-ttu-id="b0d71-202">Ação: SendSMSAlertToRecipients</span><span class="sxs-lookup"><span data-stu-id="b0d71-202">Action:SendSMSAlertToRecipients</span></span>
    
- <span data-ttu-id="b0d71-203">Ação: ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="b0d71-203">Action:ServerReplyWithMessage</span></span>
    
- <span data-ttu-id="b0d71-204">Ação: StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="b0d71-204">Action:StopProcessingRules</span></span>
    
- <span data-ttu-id="b0d71-205">IsEnabled</span><span class="sxs-lookup"><span data-stu-id="b0d71-205">IsEnabled</span></span>
    
- <span data-ttu-id="b0d71-206">IsInError</span><span class="sxs-lookup"><span data-stu-id="b0d71-206">IsInError</span></span>
    
- <span data-ttu-id="b0d71-207">Condições</span><span class="sxs-lookup"><span data-stu-id="b0d71-207">Conditions</span></span>
    
- <span data-ttu-id="b0d71-208">Exceções</span><span class="sxs-lookup"><span data-stu-id="b0d71-208">Exceptions</span></span>
    
## <a name="remarks"></a><span data-ttu-id="b0d71-209">Comentários</span><span class="sxs-lookup"><span data-stu-id="b0d71-209">Remarks</span></span>

<span data-ttu-id="b0d71-210">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0d71-210">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0d71-211">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b0d71-211">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0d71-212">Namespace</span><span class="sxs-lookup"><span data-stu-id="b0d71-212">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b0d71-213">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b0d71-213">Schema Name</span></span>  <br/> |<span data-ttu-id="b0d71-214">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="b0d71-214">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b0d71-215">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b0d71-215">Validation File</span></span>  <br/> |<span data-ttu-id="b0d71-216">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b0d71-216">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b0d71-217">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b0d71-217">Can be Empty</span></span>  <br/> |<span data-ttu-id="b0d71-218">False</span><span class="sxs-lookup"><span data-stu-id="b0d71-218">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0d71-219">Ver também</span><span class="sxs-lookup"><span data-stu-id="b0d71-219">See also</span></span>



- [<span data-ttu-id="b0d71-220">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b0d71-220">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

