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
description: O elemento de ações representa o conjunto de ações que estão disponíveis a ser executada em uma mensagem quando as condições são atendidas.
ms.openlocfilehash: 093d2f28135c6077b6cea488591573af0182934b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751040"
---
# <a name="actions"></a><span data-ttu-id="5ea2e-103">Ações</span><span class="sxs-lookup"><span data-stu-id="5ea2e-103">Actions</span></span>

<span data-ttu-id="5ea2e-104">O elemento de **ações** representa o conjunto de ações que estão disponíveis a ser executada em uma mensagem quando as condições são atendidas.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-104">The **Actions** element represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span> 
  
[<span data-ttu-id="5ea2e-105">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="5ea2e-105">Rule (RuleType)</span></span>](rule-ruletype.md)
  
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

 <span data-ttu-id="5ea2e-106">**RuleActionsType**</span><span class="sxs-lookup"><span data-stu-id="5ea2e-106">**RuleActionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5ea2e-107">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5ea2e-107">Attributes and elements</span></span>

<span data-ttu-id="5ea2e-108">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5ea2e-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="5ea2e-109">Attributes</span></span>

<span data-ttu-id="5ea2e-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5ea2e-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5ea2e-111">Child elements</span></span>

|<span data-ttu-id="5ea2e-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5ea2e-112">**Element**</span></span>|<span data-ttu-id="5ea2e-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5ea2e-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ea2e-114">AssignCategories</span><span class="sxs-lookup"><span data-stu-id="5ea2e-114">AssignCategories</span></span>](assigncategories.md) <br/> |<span data-ttu-id="5ea2e-115">Representa as categorias que estão marcadas em mensagens de email.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-115">Represents the categories that are stamped on e-mail messages.</span></span>  <br/> |
|[<span data-ttu-id="5ea2e-116">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="5ea2e-116">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="5ea2e-117">Identifica a ID da pasta que serão copiados para itens de email.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-117">Identifies the ID of the folder that e-mail items will be copied to.</span></span>  <br/> |
|[<span data-ttu-id="5ea2e-118">Delete</span><span class="sxs-lookup"><span data-stu-id="5ea2e-118">Delete</span></span>](delete.md) <br/> |<span data-ttu-id="5ea2e-119">Indica se as mensagens devem ser movidos para a pasta Itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-119">Indicates whether messages are to be moved to the Deleted Items folder.</span></span>  <br/> |
|[<span data-ttu-id="5ea2e-120">ForwardAsAttachmentToRecipients</span><span class="sxs-lookup"><span data-stu-id="5ea2e-120">ForwardAsAttachmentToRecipients</span></span>](forwardasattachmenttorecipients.md) <br/> |<span data-ttu-id="5ea2e-121">Indica os endereços de email ao qual as mensagens devem ser encaminhadas como anexos.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-121">Indicates the e-mail addresses to which messages are to be forwarded as attachments.</span></span>  <br/> |
|[<span data-ttu-id="5ea2e-122">ForwardToRecipients</span><span class="sxs-lookup"><span data-stu-id="5ea2e-122">ForwardToRecipients</span></span>](forwardtorecipients.md) <br/> |<span data-ttu-id="5ea2e-123">Indica os endereços de email ao qual as mensagens devem ser encaminhadas.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-123">Indicates the e-mail addresses to which messages are to be forwarded.</span></span>  <br/> |
|[<span data-ttu-id="5ea2e-124">MarkImportance</span><span class="sxs-lookup"><span data-stu-id="5ea2e-124">MarkImportance</span></span>](markimportance.md) <br/> |<span data-ttu-id="5ea2e-125">Especifica a importância que deve ser marcada em mensagens.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-125">Specifies the importance that is to be stamped on messages.</span></span>  <br/> |
|[<span data-ttu-id="5ea2e-126">MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="5ea2e-126">MarkAsRead</span></span>](markasread.md) <br/> |<span data-ttu-id="5ea2e-127">Indica se as mensagens devem ser marcados como lidos.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-127">Indicates whether messages are to be marked as read.</span></span>  <br/> |
|[<span data-ttu-id="5ea2e-128">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="5ea2e-128">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="5ea2e-129">Identifica a ID da pasta que serão movidos para itens de email.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-129">Identifies the ID of the folder that e-mail items will be moved to.</span></span>  <br/> |
|[<span data-ttu-id="5ea2e-130">PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="5ea2e-130">PermanentDelete</span></span>](permanentdelete.md) <br/> |<span data-ttu-id="5ea2e-131">Indica se as mensagens devem ser excluídos permanentemente e não são salvas na pasta Itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-131">Indicates whether messages are to be permanently deleted and not saved to the Deleted Items folder.</span></span>  <br/> |
|[<span data-ttu-id="5ea2e-132">RedirectToRecipients</span><span class="sxs-lookup"><span data-stu-id="5ea2e-132">RedirectToRecipients</span></span>](redirecttorecipients.md) <br/> |<span data-ttu-id="5ea2e-133">Indica os endereços de email para os quais as mensagens devem ser redirecionados.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-133">Indicates the e-mail addresses to which messages are to be redirected.</span></span>  <br/> |
|[<span data-ttu-id="5ea2e-134">SendSMSAlertToRecipients</span><span class="sxs-lookup"><span data-stu-id="5ea2e-134">SendSMSAlertToRecipients</span></span>](sendsmsalerttorecipients.md) <br/> |<span data-ttu-id="5ea2e-135">Indica os números de telefone celular para o qual um alerta do serviço SMS (Short Message) será enviado.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-135">Indicates the mobile phone numbers to which a Short Message Service (SMS) alert is to be sent.</span></span>  <br/> |
|[<span data-ttu-id="5ea2e-136">ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="5ea2e-136">ServerReplyWithMessage</span></span>](serverreplywithmessage.md) <br/> |<span data-ttu-id="5ea2e-137">Indica.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-137">Indicates.</span></span> <span data-ttu-id="5ea2e-138">a ID da mensagem modelo que deve ser enviado como uma resposta às mensagens de entrada.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-138">the ID of the template message that is to be sent as a reply to incoming messages.</span></span>  <br/> |
|[<span data-ttu-id="5ea2e-139">StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="5ea2e-139">StopProcessingRules</span></span>](stopprocessingrules.md) <br/> |<span data-ttu-id="5ea2e-140">Indica se as regras subsequentes devem ser avaliadas.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-140">Indicates whether subsequent rules are to be evaluated.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5ea2e-141">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5ea2e-141">Parent elements</span></span>

|<span data-ttu-id="5ea2e-142">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5ea2e-142">**Element**</span></span>|<span data-ttu-id="5ea2e-143">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5ea2e-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ea2e-144">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="5ea2e-144">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="5ea2e-145">Representa uma única regra na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-145">Represents a single rule in a user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5ea2e-146">Text value</span><span class="sxs-lookup"><span data-stu-id="5ea2e-146">Text value</span></span>

<span data-ttu-id="5ea2e-147">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-147">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5ea2e-148">Comentários</span><span class="sxs-lookup"><span data-stu-id="5ea2e-148">Remarks</span></span>

<span data-ttu-id="5ea2e-149">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5ea2e-149">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5ea2e-150">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5ea2e-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5ea2e-151">Namespace</span><span class="sxs-lookup"><span data-stu-id="5ea2e-151">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5ea2e-152">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5ea2e-152">Schema Name</span></span>  <br/> |<span data-ttu-id="5ea2e-153">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5ea2e-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="5ea2e-154">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5ea2e-154">Validation File</span></span>  <br/> |<span data-ttu-id="5ea2e-155">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5ea2e-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5ea2e-156">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5ea2e-156">Can be Empty</span></span>  <br/> |<span data-ttu-id="5ea2e-157">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="5ea2e-157">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5ea2e-158">Ver também</span><span class="sxs-lookup"><span data-stu-id="5ea2e-158">See also</span></span>

- [<span data-ttu-id="5ea2e-159">Condições</span><span class="sxs-lookup"><span data-stu-id="5ea2e-159">Conditions</span></span>](conditions.md)
- [<span data-ttu-id="5ea2e-160">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5ea2e-160">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

