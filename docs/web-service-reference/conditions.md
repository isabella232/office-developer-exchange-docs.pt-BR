---
title: Condições
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Conditions
api_type:
- schema
ms.assetid: f049a48c-9585-43f7-8549-0b8cb19a5eea
description: O elemento Conditions identifica as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.
ms.openlocfilehash: 2c6b4794a87cca79b4c723197b57360ad0ff973d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463199"
---
# <a name="conditions"></a><span data-ttu-id="4ac64-103">Condições</span><span class="sxs-lookup"><span data-stu-id="4ac64-103">Conditions</span></span>

<span data-ttu-id="4ac64-104">O elemento **Conditions** identifica as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="4ac64-104">The **Conditions** element identifies the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span> 
  
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

 <span data-ttu-id="4ac64-105">**RulePredicatesType**</span><span class="sxs-lookup"><span data-stu-id="4ac64-105">**RulePredicatesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ac64-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4ac64-106">Attributes and elements</span></span>

<span data-ttu-id="4ac64-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4ac64-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ac64-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4ac64-108">Attributes</span></span>

<span data-ttu-id="4ac64-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ac64-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ac64-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4ac64-110">Child elements</span></span>

|<span data-ttu-id="4ac64-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4ac64-111">**Element**</span></span>|<span data-ttu-id="4ac64-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4ac64-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ac64-113">Categories</span><span class="sxs-lookup"><span data-stu-id="4ac64-113">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="4ac64-114">Contém as categorias que devem ser aplicadas a uma mensagem de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-114">Contains the categories that must be applied to an incoming message in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-115">ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="4ac64-115">ContainsBodyStrings</span></span>](containsbodystrings.md) <br/> |<span data-ttu-id="4ac64-116">Indica as cadeias de caracteres que devem aparecer no corpo das mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-116">Indicates the strings that must appear in the body of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-117">ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="4ac64-117">ContainsHeaderStrings</span></span>](containsheaderstrings.md) <br/> |<span data-ttu-id="4ac64-118">Indica as cadeias de caracteres que devem aparecer nos cabeçalhos das mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-118">Indicates the strings that must appear in the headers of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-119">ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="4ac64-119">ContainsRecipientStrings</span></span>](containsrecipientstrings.md) <br/> |<span data-ttu-id="4ac64-120">Indica as cadeias de caracteres que devem aparecer nas propriedades **ToRecipients** ou **CcRecipients** de mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-120">Indicates the strings that must appear in either the **ToRecipients** or **CcRecipients** properties of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-121">ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="4ac64-121">ContainsSenderStrings</span></span>](containssenderstrings.md) <br/> |<span data-ttu-id="4ac64-122">Indica as cadeias de caracteres que devem aparecer na propriedade **from** de mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-122">Indicates the strings that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-123">ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="4ac64-123">ContainsSubjectOrBodyStrings</span></span>](containssubjectorbodystrings.md) <br/> |<span data-ttu-id="4ac64-124">Indica as cadeias de caracteres que devem aparecer no corpo ou no assunto das mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-124">Indicates the strings that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-125">ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="4ac64-125">ContainsSubjectStrings</span></span>](containssubjectstrings.md) <br/> |<span data-ttu-id="4ac64-126">Indica as cadeias de caracteres que devem aparecer no assunto das mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-126">Indicates the strings that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-127">FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="4ac64-127">FlaggedForAction</span></span>](flaggedforaction.md) <br/> |<span data-ttu-id="4ac64-128">Especifica o sinalizador para o valor de ação que deve aparecer nas mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-128">Specifies the flag for action value that must appear on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-129">FromAddresses</span><span class="sxs-lookup"><span data-stu-id="4ac64-129">FromAddresses</span></span>](fromaddresses.md) <br/> |<span data-ttu-id="4ac64-130">Indica os endereços de email dos quais as mensagens de entrada devem ser enviadas para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-130">Indicates the e-mail addresses from which incoming messages must be sent in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-131">FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="4ac64-131">FromConnectedAccounts</span></span>](fromconnectedaccounts.md) <br/> |<span data-ttu-id="4ac64-132">Representa os nomes das contas de email a partir das quais as mensagens de entrada precisam ser agregadas para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-132">Represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-133">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="4ac64-133">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="4ac64-134">Indica se as mensagens de entrada precisam ter anexos para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-134">Indicates whether incoming messages have to have attachments in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-135">Importance</span><span class="sxs-lookup"><span data-stu-id="4ac64-135">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="4ac64-136">Especifica a importância que é carimbada nas mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-136">Specifies the importance that is stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-137">IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="4ac64-137">IsApprovalRequest</span></span>](isapprovalrequest.md) <br/> |<span data-ttu-id="4ac64-138">Indica se as mensagens de entrada devem ser solicitações de aprovação para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-138">Indicates whether incoming messages must be approval requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-139">IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="4ac64-139">IsAutomaticForward</span></span>](isautomaticforward.md) <br/> |<span data-ttu-id="4ac64-140">Indica se as mensagens de entrada devem ser encaminhamentos automáticos para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-140">Indicates whether incoming messages must be automatic forwards in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-141">IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="4ac64-141">IsAutomaticReply</span></span>](isautomaticreply.md) <br/> |<span data-ttu-id="4ac64-142">Indica se as mensagens de entrada devem ser respostas automáticas para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-142">Indicates whether incoming messages must be automatic replies in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-143">IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="4ac64-143">IsEncrypted</span></span>](isencrypted.md) <br/> |<span data-ttu-id="4ac64-144">Indica se as mensagens de entrada devem ser criptografadas por S/MIME para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-144">Indicates whether incoming messages must be S/MIME encrypted in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-145">IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="4ac64-145">IsMeetingRequest</span></span>](ismeetingrequest.md) <br/> |<span data-ttu-id="4ac64-146">Indica se as mensagens de entrada devem ser solicitações de reunião para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-146">Indicates whether incoming messages must be meeting requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-147">IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="4ac64-147">IsMeetingResponse</span></span>](ismeetingresponse.md) <br/> |<span data-ttu-id="4ac64-148">Indica se as mensagens de entrada devem ser respostas de reunião para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-148">Indicates whether incoming messages must be meeting responses in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-149">IsNDR</span><span class="sxs-lookup"><span data-stu-id="4ac64-149">IsNDR</span></span>](isndr.md) <br/> |<span data-ttu-id="4ac64-150">Indica se as mensagens de entrada devem ser notificações de falha na entrega (NDRs) para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-150">Indicates whether incoming messages must be non-delivery reports (NDRs) in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-151">IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="4ac64-151">IsPermissionControlled</span></span>](ispermissioncontrolled.md) <br/> |<span data-ttu-id="4ac64-152">Indica se as mensagens de entrada devem ser controladas por permissões (protegidas por RMS) para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-152">Indicates whether incoming messages must be permission controlled (RMS protected) in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-153">IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="4ac64-153">IsReadReceipt</span></span>](isreadreceipt.md) <br/> |<span data-ttu-id="4ac64-154">Indica se as mensagens de entrada devem ser recibos de leitura para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-154">Indicates whether incoming messages must be read receipts in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-155">IsSigned</span><span class="sxs-lookup"><span data-stu-id="4ac64-155">IsSigned</span></span>](issigned.md) <br/> |<span data-ttu-id="4ac64-156">Indica se as mensagens de entrada devem ser assinadas por S/MIME para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-156">Indicates whether incoming messages must be S/MIME signed in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-157">Iscaixa postal</span><span class="sxs-lookup"><span data-stu-id="4ac64-157">IsVoicemail</span></span>](isvoicemail.md) <br/> |<span data-ttu-id="4ac64-158">Indica se as mensagens de entrada devem ser mensagens de caixa postal para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-158">Indicates whether incoming messages must be voice mail messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-159">Doclasss</span><span class="sxs-lookup"><span data-stu-id="4ac64-159">ItemClasses</span></span>](itemclasses.md) <br/> |<span data-ttu-id="4ac64-160">Representa as classes de item que devem ser carimbadas nas mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-160">Represents the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-161">MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="4ac64-161">MessageClassifications</span></span>](messageclassifications.md) <br/> |<span data-ttu-id="4ac64-162">Representa as classificações de mensagens que devem ser carimbadas nas mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-162">Represents the message classifications that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-163">NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="4ac64-163">NotSentToMe</span></span>](notsenttome.md) <br/> |<span data-ttu-id="4ac64-164">Indica se o proprietário da caixa de correio não deve estar na propriedade **ToRecipients** das mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-164">Indicates whether the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-165">SentCcMe</span><span class="sxs-lookup"><span data-stu-id="4ac64-165">SentCcMe</span></span>](sentccme.md) <br/> |<span data-ttu-id="4ac64-166">Indica se o proprietário da caixa de correio deve estar na propriedade **CcRecipients** de mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-166">Indicates whether the owner of the mailbox has to be in the **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-167">SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="4ac64-167">SentOnlyToMe</span></span>](sentonlytome.md) <br/> |<span data-ttu-id="4ac64-168">Indica se o proprietário da caixa de correio deve ser a única na propriedade **ToRecipients** de mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-168">Indicates whether the owner of the mailbox has to be the only one in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-169">SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="4ac64-169">SentToAddresses</span></span>](senttoaddresses.md) <br/> |<span data-ttu-id="4ac64-170">Indica os endereços de email para os quais as mensagens de entrada devem ter sido enviadas para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-170">Indicates the e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-171">SentToMe</span><span class="sxs-lookup"><span data-stu-id="4ac64-171">SentToMe</span></span>](senttome.md) <br/> |<span data-ttu-id="4ac64-172">Indica se o proprietário da caixa de correio deve estar na propriedade **ToRecipients** de mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-172">Indicates whether the owner of the mailbox has to be in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-173">SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="4ac64-173">SentToOrCcMe</span></span>](senttoorccme.md) <br/> |<span data-ttu-id="4ac64-174">Indica se o proprietário da caixa de correio deve estar em uma propriedade **ToRecipients** ou **CcRecipients** de mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-174">Indicates whether the owner of the mailbox has to be in either a **ToRecipients** or **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-175">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="4ac64-175">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="4ac64-176">Indica a sensibilidade que deve ser carimbada nas mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-176">Indicates the sensitivity that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-177">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="4ac64-177">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="4ac64-178">Especifica o intervalo de datas no qual as mensagens de entrada precisam ser recebidas para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-178">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4ac64-179">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="4ac64-179">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="4ac64-180">Especifica os tamanhos mínimo e máximo que as mensagens de entrada devem ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4ac64-180">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4ac64-181">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4ac64-181">Parent elements</span></span>

|<span data-ttu-id="4ac64-182">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4ac64-182">**Element**</span></span>|<span data-ttu-id="4ac64-183">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4ac64-183">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ac64-184">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="4ac64-184">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="4ac64-185">Contém uma única regra e representa uma regra na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4ac64-185">Contains a single rule and represents a rule in a user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4ac64-186">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="4ac64-186">Text value</span></span>

<span data-ttu-id="4ac64-187">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4ac64-187">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4ac64-188">Comentários</span><span class="sxs-lookup"><span data-stu-id="4ac64-188">Remarks</span></span>

<span data-ttu-id="4ac64-189">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ac64-189">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ac64-190">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4ac64-190">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ac64-191">Namespace</span><span class="sxs-lookup"><span data-stu-id="4ac64-191">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4ac64-192">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4ac64-192">Schema Name</span></span>  <br/> |<span data-ttu-id="4ac64-193">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4ac64-193">Types schema</span></span>  <br/> |
|<span data-ttu-id="4ac64-194">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4ac64-194">Validation File</span></span>  <br/> |<span data-ttu-id="4ac64-195">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4ac64-195">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4ac64-196">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4ac64-196">Can be Empty</span></span>  <br/> |<span data-ttu-id="4ac64-197">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="4ac64-197">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ac64-198">Confira também</span><span class="sxs-lookup"><span data-stu-id="4ac64-198">See also</span></span>



[<span data-ttu-id="4ac64-199">Exceções</span><span class="sxs-lookup"><span data-stu-id="4ac64-199">Exceptions</span></span>](exceptions.md)


- [<span data-ttu-id="4ac64-200">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4ac64-200">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

