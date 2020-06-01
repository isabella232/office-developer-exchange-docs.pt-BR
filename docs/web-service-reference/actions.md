---
title: Ações
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Actions
api_type:
- schema
ms.assetid: c5aa96b1-2d8b-422f-8c2f-f118572ab23f
description: O elemento Actions representa o conjunto de ações que estão disponíveis para serem realizadas em uma mensagem quando as condições forem atendidas.
ms.openlocfilehash: 2ac53778b583595fa8be07f2c5110a9e2df16eca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465062"
---
# <a name="actions"></a><span data-ttu-id="7c4a5-103">Ações</span><span class="sxs-lookup"><span data-stu-id="7c4a5-103">Actions</span></span>

<span data-ttu-id="7c4a5-104">O elemento **Actions** representa o conjunto de ações que estão disponíveis para serem realizadas em uma mensagem quando as condições forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="7c4a5-104">The **Actions** element represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span> 
  
[<span data-ttu-id="7c4a5-105">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="7c4a5-105">Rule (RuleType)</span></span>](rule-ruletype.md)
  
```XML
<Actions>
    <AssignCategories>
    <CopyToFolder>
    <Delete>
    <ForwardAsAttachmentToRecipients>
    <ForwardToRecipients>
    <MarkImportance>
    <MarkAsRead>
    <MoveToFolder>
    <PermanentDelete>
    <RedirectToRecipients>
    <SendSMSAlertToRecipients>
    <ServerReplyWithMessage>
    <StopProcessingRules>
</Actions>
```

 <span data-ttu-id="7c4a5-106">**RuleActionsType**</span><span class="sxs-lookup"><span data-stu-id="7c4a5-106">**RuleActionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c4a5-107">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="7c4a5-107">Attributes and elements</span></span>

<span data-ttu-id="7c4a5-108">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7c4a5-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c4a5-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="7c4a5-109">Attributes</span></span>

<span data-ttu-id="7c4a5-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7c4a5-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c4a5-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7c4a5-111">Child elements</span></span>

|<span data-ttu-id="7c4a5-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7c4a5-112">**Element**</span></span>|<span data-ttu-id="7c4a5-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7c4a5-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c4a5-114">AssignCategories</span><span class="sxs-lookup"><span data-stu-id="7c4a5-114">AssignCategories</span></span>](assigncategories.md) <br/> |<span data-ttu-id="7c4a5-115">Representa as categorias carimbadas nas mensagens de email.</span><span class="sxs-lookup"><span data-stu-id="7c4a5-115">Represents the categories that are stamped on e-mail messages.</span></span>  <br/> |
|[<span data-ttu-id="7c4a5-116">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="7c4a5-116">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="7c4a5-117">Identifica a ID da pasta para a qual os itens de email serão copiados.</span><span class="sxs-lookup"><span data-stu-id="7c4a5-117">Identifies the ID of the folder that e-mail items will be copied to.</span></span>  <br/> |
|[<span data-ttu-id="7c4a5-118">Delete</span><span class="sxs-lookup"><span data-stu-id="7c4a5-118">Delete</span></span>](delete.md) <br/> |<span data-ttu-id="7c4a5-119">Indica se as mensagens devem ser movidas para a pasta itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="7c4a5-119">Indicates whether messages are to be moved to the Deleted Items folder.</span></span>  <br/> |
|[<span data-ttu-id="7c4a5-120">ForwardAsAttachmentToRecipients</span><span class="sxs-lookup"><span data-stu-id="7c4a5-120">ForwardAsAttachmentToRecipients</span></span>](forwardasattachmenttorecipients.md) <br/> |<span data-ttu-id="7c4a5-121">Indica os endereços de email para os quais as mensagens devem ser encaminhadas como anexos.</span><span class="sxs-lookup"><span data-stu-id="7c4a5-121">Indicates the e-mail addresses to which messages are to be forwarded as attachments.</span></span>  <br/> |
|[<span data-ttu-id="7c4a5-122">ForwardToRecipients</span><span class="sxs-lookup"><span data-stu-id="7c4a5-122">ForwardToRecipients</span></span>](forwardtorecipients.md) <br/> |<span data-ttu-id="7c4a5-123">Indica os endereços de email para os quais as mensagens devem ser encaminhadas.</span><span class="sxs-lookup"><span data-stu-id="7c4a5-123">Indicates the e-mail addresses to which messages are to be forwarded.</span></span>  <br/> |
|[<span data-ttu-id="7c4a5-124">MarkImportance</span><span class="sxs-lookup"><span data-stu-id="7c4a5-124">MarkImportance</span></span>](markimportance.md) <br/> |<span data-ttu-id="7c4a5-125">Especifica a importância a ser carimbada nas mensagens.</span><span class="sxs-lookup"><span data-stu-id="7c4a5-125">Specifies the importance that is to be stamped on messages.</span></span>  <br/> |
|[<span data-ttu-id="7c4a5-126">MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="7c4a5-126">MarkAsRead</span></span>](markasread.md) <br/> |<span data-ttu-id="7c4a5-127">Indica se as mensagens devem ser marcadas como lidas.</span><span class="sxs-lookup"><span data-stu-id="7c4a5-127">Indicates whether messages are to be marked as read.</span></span>  <br/> |
|[<span data-ttu-id="7c4a5-128">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="7c4a5-128">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="7c4a5-129">Identifica a ID da pasta para a qual os itens de email serão movidos.</span><span class="sxs-lookup"><span data-stu-id="7c4a5-129">Identifies the ID of the folder that e-mail items will be moved to.</span></span>  <br/> |
|[<span data-ttu-id="7c4a5-130">PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="7c4a5-130">PermanentDelete</span></span>](permanentdelete.md) <br/> |<span data-ttu-id="7c4a5-131">Indica se as mensagens devem ser excluídas permanentemente e não são salvas na pasta itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="7c4a5-131">Indicates whether messages are to be permanently deleted and not saved to the Deleted Items folder.</span></span>  <br/> |
|[<span data-ttu-id="7c4a5-132">RedirectToRecipients</span><span class="sxs-lookup"><span data-stu-id="7c4a5-132">RedirectToRecipients</span></span>](redirecttorecipients.md) <br/> |<span data-ttu-id="7c4a5-133">Indica os endereços de email aos quais as mensagens devem ser redirecionadas.</span><span class="sxs-lookup"><span data-stu-id="7c4a5-133">Indicates the e-mail addresses to which messages are to be redirected.</span></span>  <br/> |
|[<span data-ttu-id="7c4a5-134">SendSMSAlertToRecipients</span><span class="sxs-lookup"><span data-stu-id="7c4a5-134">SendSMSAlertToRecipients</span></span>](sendsmsalerttorecipients.md) <br/> |<span data-ttu-id="7c4a5-135">Indica os números de telefone celular para os quais um alerta de serviço de mensagem curta (SMS) deve ser enviado.</span><span class="sxs-lookup"><span data-stu-id="7c4a5-135">Indicates the mobile phone numbers to which a Short Message Service (SMS) alert is to be sent.</span></span>  <br/> |
|[<span data-ttu-id="7c4a5-136">ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="7c4a5-136">ServerReplyWithMessage</span></span>](serverreplywithmessage.md) <br/> |<span data-ttu-id="7c4a5-137">Informa.</span><span class="sxs-lookup"><span data-stu-id="7c4a5-137">Indicates.</span></span> <span data-ttu-id="7c4a5-138">a ID da mensagem de modelo a ser enviada como uma resposta a mensagens de entrada.</span><span class="sxs-lookup"><span data-stu-id="7c4a5-138">the ID of the template message that is to be sent as a reply to incoming messages.</span></span>  <br/> |
|[<span data-ttu-id="7c4a5-139">StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="7c4a5-139">StopProcessingRules</span></span>](stopprocessingrules.md) <br/> |<span data-ttu-id="7c4a5-140">Indica se as regras subsequentes serão avaliadas.</span><span class="sxs-lookup"><span data-stu-id="7c4a5-140">Indicates whether subsequent rules are to be evaluated.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7c4a5-141">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7c4a5-141">Parent elements</span></span>

|<span data-ttu-id="7c4a5-142">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7c4a5-142">**Element**</span></span>|<span data-ttu-id="7c4a5-143">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7c4a5-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c4a5-144">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="7c4a5-144">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="7c4a5-145">Representa uma única regra na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="7c4a5-145">Represents a single rule in a user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7c4a5-146">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="7c4a5-146">Text value</span></span>

<span data-ttu-id="7c4a5-147">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7c4a5-147">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7c4a5-148">Comentários</span><span class="sxs-lookup"><span data-stu-id="7c4a5-148">Remarks</span></span>

<span data-ttu-id="7c4a5-149">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7c4a5-149">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c4a5-150">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="7c4a5-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c4a5-151">Namespace</span><span class="sxs-lookup"><span data-stu-id="7c4a5-151">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c4a5-152">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7c4a5-152">Schema Name</span></span>  <br/> |<span data-ttu-id="7c4a5-153">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7c4a5-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="7c4a5-154">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7c4a5-154">Validation File</span></span>  <br/> |<span data-ttu-id="7c4a5-155">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7c4a5-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c4a5-156">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7c4a5-156">Can be Empty</span></span>  <br/> |<span data-ttu-id="7c4a5-157">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="7c4a5-157">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c4a5-158">Também consulte</span><span class="sxs-lookup"><span data-stu-id="7c4a5-158">See also</span></span>

- [<span data-ttu-id="7c4a5-159">Condições</span><span class="sxs-lookup"><span data-stu-id="7c4a5-159">Conditions</span></span>](conditions.md)
- [<span data-ttu-id="7c4a5-160">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7c4a5-160">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

