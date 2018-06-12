---
title: Operação UpdateInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateInboxRules
api_type:
- schema
ms.assetid: f982a237-471e-45c5-a2b5-468cfc53150b
description: A operação UpdateInboxRules atualiza regras de caixa de entrada do usuário autenticado, aplicando as operações especificadas. UpdateInboxRules é usado para criar uma regra de caixa de entrada, para definir uma regra de caixa de correio ou para excluir uma regra de caixa de entrada.
ms.openlocfilehash: 6e979421d619fed6625fe05db86c1f8c6a7418c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837903"
---
# <a name="updateinboxrules-operation"></a><span data-ttu-id="4fbfe-104">Operação UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="4fbfe-104">UpdateInboxRules operation</span></span>

<span data-ttu-id="4fbfe-105">A operação UpdateInboxRules atualiza regras de caixa de entrada do usuário autenticado, aplicando as operações especificadas.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-105">The UpdateInboxRules operation updates the authenticated user's Inbox rules by applying the specified operations.</span></span> <span data-ttu-id="4fbfe-106">**UpdateInboxRules** é usado para criar uma regra de caixa de entrada, para definir uma regra de caixa de correio ou para excluir uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-106">**UpdateInboxRules** is used to create an Inbox rule, to set an Inbox rule, or to delete an Inbox rule.</span></span> 
  
<span data-ttu-id="4fbfe-107">Quando você usar a operação **UpdateInboxRules** , serviços Web do Exchange exclui regras de envio do lado do cliente.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-107">When you use the **UpdateInboxRules** operation, Exchange Web Services deletes client-side send rules.</span></span> <span data-ttu-id="4fbfe-108">Regras de envio do lado do cliente são armazenadas no cliente na regra de mensagem de informações de associado de pasta (FAI) e em nenhum outro lugar.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-108">Client-side send rules are stored on the client in the rule Folder Associated Information (FAI) Message and nowhere else.</span></span> <span data-ttu-id="4fbfe-109">EWS exclui essa regra mensagem FAI por padrão, com base na expectativa de que o Outlook irá recriá-lo.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-109">EWS deletes this rule FAI message by default, based on the expectation that Outlook will recreate it.</span></span> <span data-ttu-id="4fbfe-110">No entanto, Outlook não puder recriar as regras que não existem também como uma regra estendida e regras de envio do lado do cliente não existirem como regras estendidas.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-110">However, Outlook can't recreate rules that don't also exist as an extended rule, and client-side send rules don't exist as extended rules.</span></span> <span data-ttu-id="4fbfe-111">Como resultado, essas regras são perdidas.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-111">As a result, these rules are lost.</span></span> <span data-ttu-id="4fbfe-112">Sugerimos que você considere o seguinte ao projetar sua solução.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-112">We suggest you consider this when designing your solution.</span></span> 
  
## <a name="updateinboxrules-create-rule-request-example"></a><span data-ttu-id="4fbfe-113">Exemplo de solicitação de UpdateInboxRules (Criar regra)</span><span class="sxs-lookup"><span data-stu-id="4fbfe-113">UpdateInboxRules (Create Rule) request example</span></span>

<span data-ttu-id="4fbfe-114">Você pode usar os serviços Web do Exchange para criar uma regra de caixa de entrada na caixa de correio do usuário no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-114">You can use Exchange Web Services to create an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="4fbfe-115">Use o elemento [UpdateInboxRules](updateinboxrules.md) em conjunto com o elemento [CreateRuleOperation](createruleoperation.md) para criar uma regra.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-115">Use the [UpdateInboxRules](updateinboxrules.md) element in conjunction with the [CreateRuleOperation](createruleoperation.md) element to create a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="4fbfe-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fbfe-116">Description</span></span>

<span data-ttu-id="4fbfe-117">O cliente constrói solicitação XML e o envia ao servidor.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-117">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="4fbfe-118">Código</span><span class="sxs-lookup"><span data-stu-id="4fbfe-118">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <m:Operations>
          <t:CreateRuleOperation>
            <t:Rule>
              <t:DisplayName>MoveInterestingToJunk</t:DisplayName>
              <t:Priority>1</t:Priority>
              <t:IsEnabled>true</t:IsEnabled>
              <t:Conditions>
                <t:ContainsSubjectStrings>
                  <t:String>Interesting</t:String>
                </t:ContainsSubjectStrings>
              </t:Conditions>
              <t:Exceptions />
              <t:Actions>
                <t:MoveToFolder>
                  <t:DistinguishedFolderId Id="junkemail" />
                </t:MoveToFolder>
              </t:Actions>
            </t:Rule>
          </t:CreateRuleOperation>
        </m:Operations>
      </m:UpdateInboxRules>
  </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a><span data-ttu-id="4fbfe-119">Comments</span><span class="sxs-lookup"><span data-stu-id="4fbfe-119">Comments</span></span>

<span data-ttu-id="4fbfe-120">Este exemplo cria uma regra que moverá uma mensagem de email para a pasta Lixo eletrônico, se o assunto do email contém uma cadeia de caracteres que é igual a "Interessante".</span><span class="sxs-lookup"><span data-stu-id="4fbfe-120">This example builds a rule that will move an e-mail message to the Junk E-mail folder if the e-mail subject contains a string that equals "Interesting".</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="4fbfe-121">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4fbfe-121">Request elements</span></span>

<span data-ttu-id="4fbfe-122">A solicitação de **UpdateInboxRules** inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="4fbfe-122">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="4fbfe-123">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="4fbfe-123">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="4fbfe-124">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="4fbfe-124">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="4fbfe-125">Operations</span><span class="sxs-lookup"><span data-stu-id="4fbfe-125">Operations</span></span>](operations.md)
    
<span data-ttu-id="4fbfe-126">O elemento de [operações](operations.md) contém o elemento [CreateRuleOperation](createruleoperation.md) para criar uma regra.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-126">The [Operations](operations.md) element contains the [CreateRuleOperation](createruleoperation.md) element to create a rule.</span></span> 
  
## <a name="updateinboxrules-create-rule-response-example"></a><span data-ttu-id="4fbfe-127">Exemplo de resposta UpdateInboxRules (Criar regra)</span><span class="sxs-lookup"><span data-stu-id="4fbfe-127">UpdateInboxRules (Create Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="4fbfe-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fbfe-128">Description</span></span>

<span data-ttu-id="4fbfe-129">O exemplo de corpo simples (SOAP Object Access Protocol) a seguir mostra uma resposta bem-sucedida à solicitação de **UpdateInboxRules** que cria uma regra.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-129">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that creates a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="4fbfe-130">Código</span><span class="sxs-lookup"><span data-stu-id="4fbfe-130">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" Version="Exchange2010_SP1" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
         ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="4fbfe-131">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="4fbfe-131">Successful response elements</span></span>

<span data-ttu-id="4fbfe-132">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="4fbfe-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="4fbfe-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4fbfe-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="4fbfe-134">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="4fbfe-134">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="4fbfe-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4fbfe-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="4fbfe-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4fbfe-136">ResponseCode</span></span>](responsecode.md)
    
## <a name="updateinboxrules-set-rule-request-example"></a><span data-ttu-id="4fbfe-137">Exemplo de solicitação de UpdateInboxRules (regra definido)</span><span class="sxs-lookup"><span data-stu-id="4fbfe-137">UpdateInboxRules (Set Rule) request example</span></span>

<span data-ttu-id="4fbfe-138">Você pode usar os serviços Web do Exchange para modificar uma regra de caixa de entrada na caixa de correio do usuário no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-138">You can use Exchange Web Services to modify an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="4fbfe-139">Use o elemento [UpdateInboxRules](updateinboxrules.md) em conjunto com o elemento [SetRuleOperation](setruleoperation.md) para modificar uma regra.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-139">Use the [UpdateInboxRules](updateinboxrules.md) element in conjunction with the [SetRuleOperation](setruleoperation.md) element to modify a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="4fbfe-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fbfe-140">Description</span></span>

<span data-ttu-id="4fbfe-141">O cliente constrói solicitação XML e o envia ao servidor.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-141">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="4fbfe-142">Código</span><span class="sxs-lookup"><span data-stu-id="4fbfe-142">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <Operations xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
          <SetRuleOperation xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
            <Rule>
              <RuleId>Nh8AAAAwW/w=</RuleId>
              <DisplayName>(Modified) This is Junk</DisplayName>
              <Priority>1</Priority>
              <IsEnabled>true</IsEnabled>
              <Conditions>
                <ContainsSubjectStrings>
                  <String>Interesting</String>
                </ContainsSubjectStrings>
              </Conditions>
              <Actions>
                <MoveToFolder>
                  <FolderId Id="AAMkADQ1YTE1" ChangeKey="AQAAAA==" />
                </MoveToFolder>
              </Actions>
            </Rule>
          </SetRuleOperation>
        </Operations>
      </m:UpdateInboxRules>
  </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a><span data-ttu-id="4fbfe-143">Comments</span><span class="sxs-lookup"><span data-stu-id="4fbfe-143">Comments</span></span>

<span data-ttu-id="4fbfe-144">Este exemplo altera o nome para exibição "(modificado) Esta é lixo".</span><span class="sxs-lookup"><span data-stu-id="4fbfe-144">This example changes the display name to "(Modified) This is Junk".</span></span>
  
> [!NOTE]
> <span data-ttu-id="4fbfe-145">Os valores de **Id** e **ChangeKey** atributos do elemento [FolderId](folderid.md) foram diminuídos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-145">The values of the **Id** and **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="4fbfe-146">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4fbfe-146">Request elements</span></span>

<span data-ttu-id="4fbfe-147">A solicitação de **UpdateInboxRules** inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="4fbfe-147">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="4fbfe-148">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="4fbfe-148">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="4fbfe-149">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="4fbfe-149">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="4fbfe-150">Operations</span><span class="sxs-lookup"><span data-stu-id="4fbfe-150">Operations</span></span>](operations.md)
    
<span data-ttu-id="4fbfe-151">O elemento de [operações](operations.md) contém o elemento [SetRuleOperation](setruleoperation.md) para modificar uma regra.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-151">The [Operations](operations.md) element contains the [SetRuleOperation](setruleoperation.md) element to modify a rule.</span></span> 
  
## <a name="updateinboxrules-set-rule-response-example"></a><span data-ttu-id="4fbfe-152">Exemplo de resposta UpdateInboxRules (regra definido)</span><span class="sxs-lookup"><span data-stu-id="4fbfe-152">UpdateInboxRules (Set Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="4fbfe-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fbfe-153">Description</span></span>

<span data-ttu-id="4fbfe-154">O exemplo de corpo simples (SOAP Object Access Protocol) a seguir mostra uma resposta bem-sucedida à solicitação de **UpdateInboxRules** que modifica uma regra.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-154">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that modifies a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="4fbfe-155">Código</span><span class="sxs-lookup"><span data-stu-id="4fbfe-155">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" 
        Version="Exchange2010_SP1" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
          ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="4fbfe-156">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="4fbfe-156">Successful response elements</span></span>

<span data-ttu-id="4fbfe-157">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="4fbfe-157">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="4fbfe-158">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4fbfe-158">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="4fbfe-159">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="4fbfe-159">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="4fbfe-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4fbfe-160">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="4fbfe-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4fbfe-161">ResponseCode</span></span>](responsecode.md)
    
## <a name="updateinboxrules-delete-rule-request-example"></a><span data-ttu-id="4fbfe-162">Exemplo de solicitação de UpdateInboxRules (Excluir regra)</span><span class="sxs-lookup"><span data-stu-id="4fbfe-162">UpdateInboxRules (Delete Rule) request example</span></span>

<span data-ttu-id="4fbfe-163">Você pode usar os serviços Web do Exchange para excluir uma regra de caixa de entrada na caixa de correio do usuário no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-163">You can use Exchange Web Services to delete an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="4fbfe-164">Use o [UpdateInboxRules](updateinboxrules.md) em conjunto com o elemento [DeleteRuleOperation](deleteruleoperation.md) para excluir uma regra.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-164">Use the [UpdateInboxRules](updateinboxrules.md) in conjunction with the [DeleteRuleOperation](deleteruleoperation.md) element to delete a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="4fbfe-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fbfe-165">Description</span></span>

<span data-ttu-id="4fbfe-166">O cliente constrói solicitação XML e o envia ao servidor.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-166">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="4fbfe-167">Código</span><span class="sxs-lookup"><span data-stu-id="4fbfe-167">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <m:Operations>
          <t:DeleteRuleOperation>
            <t:RuleId>Nh8AAAAwW/U=</t:RuleId>
          </t:DeleteRuleOperation>
        </m:Operations>
      </m:UpdateInboxRules>
  </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a><span data-ttu-id="4fbfe-168">Comments</span><span class="sxs-lookup"><span data-stu-id="4fbfe-168">Comments</span></span>

<span data-ttu-id="4fbfe-169">Este exemplo exclui a regra identificada existente.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-169">This example deletes the existing identified rule.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="4fbfe-170">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4fbfe-170">Request elements</span></span>

<span data-ttu-id="4fbfe-171">A solicitação de **UpdateInboxRules** inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="4fbfe-171">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="4fbfe-172">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="4fbfe-172">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="4fbfe-173">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="4fbfe-173">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="4fbfe-174">Operations</span><span class="sxs-lookup"><span data-stu-id="4fbfe-174">Operations</span></span>](operations.md)
    
<span data-ttu-id="4fbfe-175">O elemento de [operações](operations.md) contém o elemento [DeleteRuleOperation](deleteruleoperation.md) para excluir uma regra.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-175">The [Operations](operations.md) element contains the [DeleteRuleOperation](deleteruleoperation.md) element to delete a rule.</span></span> 
  
## <a name="updateinboxrules-delete-rule-response-example"></a><span data-ttu-id="4fbfe-176">Exemplo de resposta UpdateInboxRules (Excluir regra)</span><span class="sxs-lookup"><span data-stu-id="4fbfe-176">UpdateInboxRules (Delete Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="4fbfe-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fbfe-177">Description</span></span>

<span data-ttu-id="4fbfe-178">O exemplo de corpo simples (SOAP Object Access Protocol) a seguir mostra uma resposta bem-sucedida à solicitação de **UpdateInboxRules** que exclui uma regra.</span><span class="sxs-lookup"><span data-stu-id="4fbfe-178">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that deletes a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="4fbfe-179">Código</span><span class="sxs-lookup"><span data-stu-id="4fbfe-179">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" 
        Version="Exchange2010_SP1" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="4fbfe-180">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="4fbfe-180">Successful response elements</span></span>

<span data-ttu-id="4fbfe-181">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="4fbfe-181">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="4fbfe-182">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4fbfe-182">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="4fbfe-183">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="4fbfe-183">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="4fbfe-184">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4fbfe-184">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="4fbfe-185">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4fbfe-185">ResponseCode</span></span>](responsecode.md)
    
## <a name="see-also"></a><span data-ttu-id="4fbfe-186">Confira também</span><span class="sxs-lookup"><span data-stu-id="4fbfe-186">See also</span></span>



[<span data-ttu-id="4fbfe-187">Operação GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="4fbfe-187">GetInboxRules operation</span></span>](getinboxrules-operation.md)

