---
title: Exceções
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exceptions
api_type:
- schema
ms.assetid: 7cd63ac2-3441-4ed4-915b-6f90af4b28fc
description: O elemento de exceções identifica as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.
ms.openlocfilehash: b875b4dc0029bb9e0bc2bb50c41569fb72ef9268
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752127"
---
# <a name="exceptions"></a><span data-ttu-id="01543-103">Exceções</span><span class="sxs-lookup"><span data-stu-id="01543-103">Exceptions</span></span>

<span data-ttu-id="01543-104">O elemento de **exceções** identifica as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="01543-104">The **Exceptions** element identifies the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span> 
  
```XML
<Conditions>
   <Categories/>
   <ContainsBodyStrings/>
   <ContainsHeaderStrings/>
   <ContainsRecipientStrings/>
   <ContainsSenderStrings/>
   <ContainsSubjectOrBodyStrings/>
   <ContainsSubjectStrings/>
   <FlaggedForAction/>
   <FromAddresses/>
   <FromConnectedAccounts/>
   <HasAttachments/>
   <Importance/>
   <IsApprovalRequest/>
   <IsAutomaticForward/>
   <IsAutomaticReply/>
   <IsEncrypted/>
   <IsMeetingRequest/>
   <IsMeetingResponse/>
   <IsNDR/>
   <IsPermissionControlled/>
   <IsReadReceipt/>
   <IsSigned/>
   <IsVoicemail/>
   <ItemClasses/>
   <MessageClassifications/>
   <NotSentToMe/>
   <SentCcMe/>
   <SentOnlyToMe/>
   <SentToAddresses/>
   <SentToMe/>
   <SentToOrCcMe/>
   <Sensitivity/>
   <WithinDateRange/>
   <WithinSizeRange/>
</Conditions>
```

 <span data-ttu-id="01543-105">**RulePredicatesType**</span><span class="sxs-lookup"><span data-stu-id="01543-105">**RulePredicatesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01543-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="01543-106">Attributes and elements</span></span>

<span data-ttu-id="01543-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="01543-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01543-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="01543-108">Attributes</span></span>

<span data-ttu-id="01543-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="01543-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01543-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="01543-110">Child elements</span></span>

|<span data-ttu-id="01543-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="01543-111">**Element**</span></span>|<span data-ttu-id="01543-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="01543-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01543-113">Categories</span><span class="sxs-lookup"><span data-stu-id="01543-113">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="01543-114">Contém as categorias que devem ser aplicadas a uma mensagem de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-114">Contains the categories that must be applied to an incoming message in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-115">ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="01543-115">ContainsBodyStrings</span></span>](containsbodystrings.md) <br/> |<span data-ttu-id="01543-116">Indica as cadeias de caracteres que devem aparecer no corpo de mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-116">Indicates the strings that must appear in the body of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-117">ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="01543-117">ContainsHeaderStrings</span></span>](containsheaderstrings.md) <br/> |<span data-ttu-id="01543-118">Indicaqtes as cadeias de caracteres que devem aparecer nos cabeçalhos de mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-118">Indicaqtes the strings that must appear in the headers of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-119">ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="01543-119">ContainsRecipientStrings</span></span>](containsrecipientstrings.md) <br/> |<span data-ttu-id="01543-120">Indica as cadeias de caracteres que devem aparecer em Propriedades no **ToRecipients** ou **Cc** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-120">Indicates the strings that must appear in either the **ToRecipients** or **CcRecipients** properties of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-121">ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="01543-121">ContainsSenderStrings</span></span>](containssenderstrings.md) <br/> |<span data-ttu-id="01543-122">Indica as cadeias de caracteres que devem aparecer na propriedade **** das mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-122">Indicates the strings that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-123">ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="01543-123">ContainsSubjectOrBodyStrings</span></span>](containssubjectorbodystrings.md) <br/> |<span data-ttu-id="01543-124">Indica as cadeias de caracteres que devem aparecer no corpo ou o assunto de mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-124">Indicates the strings that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-125">ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="01543-125">ContainsSubjectStrings</span></span>](containssubjectstrings.md) <br/> |<span data-ttu-id="01543-126">Indica as cadeias de caracteres que devem aparecer no assunto do mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-126">Indicates the strings that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-127">FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="01543-127">FlaggedForAction</span></span>](flaggedforaction.md) <br/> |<span data-ttu-id="01543-128">Especifica o sinalizador para o valor de ação que deverá aparecer nas mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-128">Specifies the flag for action value that must appear on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-129">FromAddresses</span><span class="sxs-lookup"><span data-stu-id="01543-129">FromAddresses</span></span>](fromaddresses.md) <br/> |<span data-ttu-id="01543-130">Indica os endereços de email do qual as mensagens de entrada devem ser enviadas na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-130">Indicates the e-mail addresses from which incoming messages must be sent in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-131">FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="01543-131">FromConnectedAccounts</span></span>](fromconnectedaccounts.md) <br/> |<span data-ttu-id="01543-132">Representa os nomes de conta de email do qual mensagens recebidas precisam ter foram agregados na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-132">Represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-133">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="01543-133">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="01543-134">Indica se as mensagens recebidas precisam ter anexos em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-134">Indicates whether incoming messages have to have attachments in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-135">Importância</span><span class="sxs-lookup"><span data-stu-id="01543-135">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="01543-136">Especifica a importância que é marcada nas mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-136">Specifies the importance that is stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-137">IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="01543-137">IsApprovalRequest</span></span>](isapprovalrequest.md) <br/> |<span data-ttu-id="01543-138">Indica se as mensagens de entrada devem ser solicitações de aprovação em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-138">Indicates whether incoming messages must be approval requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-139">IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="01543-139">IsAutomaticForward</span></span>](isautomaticforward.md) <br/> |<span data-ttu-id="01543-140">Indica se as mensagens de entrada devem ser encaminhamentos automáticos na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-140">Indicates whether incoming messages must be automatic forwards in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-141">IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="01543-141">IsAutomaticReply</span></span>](isautomaticreply.md) <br/> |<span data-ttu-id="01543-142">Indica se as mensagens recebidas devem ser as respostas automáticas na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-142">Indicates whether incoming messages must be automatic replies in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-143">IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="01543-143">IsEncrypted</span></span>](isencrypted.md) <br/> |<span data-ttu-id="01543-144">Indica se as mensagens de entrada devem ser S/MIME criptografada em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-144">Indicates whether incoming messages must be S/MIME encrypted in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-145">IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="01543-145">IsMeetingRequest</span></span>](ismeetingrequest.md) <br/> |<span data-ttu-id="01543-146">Indica se as mensagens de entrada devem ser solicitações de reunião na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-146">Indicates whether incoming messages must be meeting requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-147">IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="01543-147">IsMeetingResponse</span></span>](ismeetingresponse.md) <br/> |<span data-ttu-id="01543-148">Indica se as mensagens de entrada devem ser respostas de reunião na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-148">Indicates whether incoming messages must be meeting responses in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-149">IsNDR</span><span class="sxs-lookup"><span data-stu-id="01543-149">IsNDR</span></span>](isndr.md) <br/> |<span data-ttu-id="01543-150">Indica se as mensagens recebidas devem ser relatórios de falha na entrega (NDRs) em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-150">Indicates whether incoming messages must be non-delivery reports (NDRs) in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-151">IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="01543-151">IsPermissionControlled</span></span>](ispermissioncontrolled.md) <br/> |<span data-ttu-id="01543-152">Indica se as mensagens de entrada devem ser controlado de permissão (protegida por RMS) na ordem para a condição ou uma exceção a ser aplicado</span><span class="sxs-lookup"><span data-stu-id="01543-152">Indicates whether incoming messages must be permission controlled (RMS protected) in order for the condition or exception to apply</span></span>  <br/> |
|[<span data-ttu-id="01543-153">IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="01543-153">IsReadReceipt</span></span>](isreadreceipt.md) <br/> |<span data-ttu-id="01543-154">Indica se as mensagens de entrada devem ser confirmações de leitura na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-154">Indicates whether incoming messages must be read receipts in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-155">IsSigned</span><span class="sxs-lookup"><span data-stu-id="01543-155">IsSigned</span></span>](issigned.md) <br/> |<span data-ttu-id="01543-156">Indica se as mensagens de entrada devem ser QUE S/MIME assinadas em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-156">Indicates whether incoming messages must be S/MIME signed in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-157">IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="01543-157">IsVoicemail</span></span>](isvoicemail.md) <br/> |<span data-ttu-id="01543-158">Indica se as mensagens de entrada devem ser mensagens de caixa postal na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-158">Indicates whether incoming messages must be voice mail messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-159">ItemClasses</span><span class="sxs-lookup"><span data-stu-id="01543-159">ItemClasses</span></span>](itemclasses.md) <br/> |<span data-ttu-id="01543-160">Representa as classes de item que devem ser marcadas em mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-160">Represents the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-161">MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="01543-161">MessageClassifications</span></span>](messageclassifications.md) <br/> |<span data-ttu-id="01543-162">Representa as classificações de mensagem que devem ser marcadas em mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-162">Represents the message classifications that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-163">NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="01543-163">NotSentToMe</span></span>](notsenttome.md) <br/> |<span data-ttu-id="01543-164">Indica se o proprietário da caixa de correio não deve ser na propriedade **ToRecipients** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-164">Indicates whether the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-165">SentCcMe</span><span class="sxs-lookup"><span data-stu-id="01543-165">SentCcMe</span></span>](sentccme.md) <br/> |<span data-ttu-id="01543-166">Indica se o proprietário da caixa de correio deve ser na propriedade **Cc** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-166">Indicates whether the owner of the mailbox has to be in the **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-167">SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="01543-167">SentOnlyToMe</span></span>](sentonlytome.md) <br/> |<span data-ttu-id="01543-168">Indica se o proprietário da caixa de correio deve ser a única pessoa na propriedade **ToRecipients** de mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-168">Indicates whether the owner of the mailbox has to be the only one in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-169">SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="01543-169">SentToAddresses</span></span>](senttoaddresses.md) <br/> |<span data-ttu-id="01543-170">Indica os endereços de email que precisam foram enviadas em ordem para a condição ou exceção para aplicar a mensagens de entrada.</span><span class="sxs-lookup"><span data-stu-id="01543-170">Indicates the e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-171">SentToMe</span><span class="sxs-lookup"><span data-stu-id="01543-171">SentToMe</span></span>](senttome.md) <br/> |<span data-ttu-id="01543-172">Indica se o proprietário da caixa de correio deve ser na propriedade **ToRecipients** de mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-172">Indicates whether the owner of the mailbox has to be in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-173">SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="01543-173">SentToOrCcMe</span></span>](senttoorccme.md) <br/> |<span data-ttu-id="01543-174">Indica se o proprietário da caixa de correio deve ser na propriedade um **ToRecipients** ou **Cc** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-174">Indicates whether the owner of the mailbox has to be in either a **ToRecipients** or **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-175">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="01543-175">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="01543-176">Indica a sensibilidade que deve ser marcada em mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-176">Indicates the sensitivity that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-177">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="01543-177">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="01543-178">Especifica o intervalo de datas dentro do qual as mensagens recebidas precisará foram recebidos em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-178">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="01543-179">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="01543-179">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="01543-180">Especifica os tamanhos mínimos e máximo que as mensagens recebidas devem estar na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="01543-180">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="01543-181">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="01543-181">Parent elements</span></span>

|<span data-ttu-id="01543-182">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="01543-182">**Element**</span></span>|<span data-ttu-id="01543-183">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="01543-183">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01543-184">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="01543-184">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="01543-185">Contém uma única regra e representa uma regra de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="01543-185">Contains a single rule and represents a rule in a user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="01543-186">Text value</span><span class="sxs-lookup"><span data-stu-id="01543-186">Text value</span></span>

<span data-ttu-id="01543-187">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="01543-187">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="01543-188">Comentários</span><span class="sxs-lookup"><span data-stu-id="01543-188">Remarks</span></span>

<span data-ttu-id="01543-189">Os predicados de regra são usados como regra condições ou exceções.</span><span class="sxs-lookup"><span data-stu-id="01543-189">The rule predicates are used as rule conditions or exceptions.</span></span>
  
<span data-ttu-id="01543-190">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="01543-190">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01543-191">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="01543-191">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01543-192">Namespace</span><span class="sxs-lookup"><span data-stu-id="01543-192">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="01543-193">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="01543-193">Schema Name</span></span>  <br/> |<span data-ttu-id="01543-194">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="01543-194">Types schema</span></span>  <br/> |
|<span data-ttu-id="01543-195">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="01543-195">Validation File</span></span>  <br/> |<span data-ttu-id="01543-196">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="01543-196">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="01543-197">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="01543-197">Can be Empty</span></span>  <br/> |<span data-ttu-id="01543-198">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="01543-198">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01543-199">Ver também</span><span class="sxs-lookup"><span data-stu-id="01543-199">See also</span></span>



[<span data-ttu-id="01543-200">Condições</span><span class="sxs-lookup"><span data-stu-id="01543-200">Conditions</span></span>](conditions.md)


- [<span data-ttu-id="01543-201">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="01543-201">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

