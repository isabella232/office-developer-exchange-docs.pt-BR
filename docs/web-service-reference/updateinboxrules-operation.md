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
description: A operação UpdateInboxRules atualiza as regras de caixa de entrada do usuário autenticado aplicando as operações especificadas. UpdateInboxRules é usado para criar uma regra de caixa de entrada, para definir uma regra de caixa de entrada, ou para excluir uma regra de caixa de entrada.
ms.openlocfilehash: a6ced4be25c6fe4649ad649ba01194791548bf67
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530997"
---
# <a name="updateinboxrules-operation"></a><span data-ttu-id="174aa-104">Operação UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="174aa-104">UpdateInboxRules operation</span></span>

<span data-ttu-id="174aa-105">A operação UpdateInboxRules atualiza as regras de caixa de entrada do usuário autenticado aplicando as operações especificadas.</span><span class="sxs-lookup"><span data-stu-id="174aa-105">The UpdateInboxRules operation updates the authenticated user's Inbox rules by applying the specified operations.</span></span> <span data-ttu-id="174aa-106">**UpdateInboxRules** é usado para criar uma regra de caixa de entrada, para definir uma regra de caixa de entrada, ou para excluir uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="174aa-106">**UpdateInboxRules** is used to create an Inbox rule, to set an Inbox rule, or to delete an Inbox rule.</span></span> 
  
<span data-ttu-id="174aa-107">Quando você usa a operação **UpdateInboxRules** , os serviços Web do Exchange excluem as regras de envio do lado do cliente.</span><span class="sxs-lookup"><span data-stu-id="174aa-107">When you use the **UpdateInboxRules** operation, Exchange Web Services deletes client-side send rules.</span></span> <span data-ttu-id="174aa-108">As regras de envio do lado do cliente são armazenadas no cliente na mensagem de FAI (informações associadas à pasta de regras) e em outro lugar.</span><span class="sxs-lookup"><span data-stu-id="174aa-108">Client-side send rules are stored on the client in the rule Folder Associated Information (FAI) Message and nowhere else.</span></span> <span data-ttu-id="174aa-109">O EWS exclui essa regra FAI mensagem por padrão, com base na expectativa de que o Outlook a recriará.</span><span class="sxs-lookup"><span data-stu-id="174aa-109">EWS deletes this rule FAI message by default, based on the expectation that Outlook will recreate it.</span></span> <span data-ttu-id="174aa-110">No entanto, o Outlook não pode recriar regras que não existam também como uma regra estendida e as regras de envio do lado do cliente não existem como regras estendidas.</span><span class="sxs-lookup"><span data-stu-id="174aa-110">However, Outlook can't recreate rules that don't also exist as an extended rule, and client-side send rules don't exist as extended rules.</span></span> <span data-ttu-id="174aa-111">Como resultado, essas regras são perdidas.</span><span class="sxs-lookup"><span data-stu-id="174aa-111">As a result, these rules are lost.</span></span> <span data-ttu-id="174aa-112">Sugerimos que você considere isso ao criar sua solução.</span><span class="sxs-lookup"><span data-stu-id="174aa-112">We suggest you consider this when designing your solution.</span></span> 
  
## <a name="updateinboxrules-create-rule-request-example"></a><span data-ttu-id="174aa-113">Exemplo de solicitação UpdateInboxRules (criar regra)</span><span class="sxs-lookup"><span data-stu-id="174aa-113">UpdateInboxRules (Create Rule) request example</span></span>

<span data-ttu-id="174aa-114">Você pode usar os serviços Web do Exchange para criar uma regra de caixa de entrada na caixa de correio de um usuário no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="174aa-114">You can use Exchange Web Services to create an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="174aa-115">Use o elemento [UpdateInboxRules](updateinboxrules.md) em conjunto com o elemento [CreateRuleOperation](createruleoperation.md) para criar uma regra.</span><span class="sxs-lookup"><span data-stu-id="174aa-115">Use the [UpdateInboxRules](updateinboxrules.md) element in conjunction with the [CreateRuleOperation](createruleoperation.md) element to create a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="174aa-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="174aa-116">Description</span></span>

<span data-ttu-id="174aa-117">O cliente cria a solicitação XML e a envia para o servidor.</span><span class="sxs-lookup"><span data-stu-id="174aa-117">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="174aa-118">Código</span><span class="sxs-lookup"><span data-stu-id="174aa-118">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="174aa-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="174aa-119">Comments</span></span>

<span data-ttu-id="174aa-120">Este exemplo cria uma regra que moverá uma mensagem de email para a pasta lixo eletrônico, se o assunto do email contiver uma cadeia de caracteres igual a "interessante".</span><span class="sxs-lookup"><span data-stu-id="174aa-120">This example builds a rule that will move an e-mail message to the Junk E-mail folder if the e-mail subject contains a string that equals "Interesting".</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="174aa-121">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="174aa-121">Request elements</span></span>

<span data-ttu-id="174aa-122">A solicitação **UpdateInboxRules** inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="174aa-122">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="174aa-123">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="174aa-123">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="174aa-124">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="174aa-124">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="174aa-125">Operations</span><span class="sxs-lookup"><span data-stu-id="174aa-125">Operations</span></span>](operations.md)
    
<span data-ttu-id="174aa-126">O elemento [Operations](operations.md) contém o elemento [CreateRuleOperation](createruleoperation.md) para criar uma regra.</span><span class="sxs-lookup"><span data-stu-id="174aa-126">The [Operations](operations.md) element contains the [CreateRuleOperation](createruleoperation.md) element to create a rule.</span></span> 
  
## <a name="updateinboxrules-create-rule-response-example"></a><span data-ttu-id="174aa-127">Exemplo de resposta UpdateInboxRules (Create Rule)</span><span class="sxs-lookup"><span data-stu-id="174aa-127">UpdateInboxRules (Create Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="174aa-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="174aa-128">Description</span></span>

<span data-ttu-id="174aa-129">O exemplo a seguir do corpo SOAP (Simple Object Access Protocol) mostra uma resposta bem-sucedida à solicitação **UpdateInboxRules** que cria uma regra.</span><span class="sxs-lookup"><span data-stu-id="174aa-129">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that creates a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="174aa-130">Código</span><span class="sxs-lookup"><span data-stu-id="174aa-130">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" Version="Exchange2010_SP1" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
         ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="174aa-131">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="174aa-131">Successful response elements</span></span>

<span data-ttu-id="174aa-132">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="174aa-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="174aa-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="174aa-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="174aa-134">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="174aa-134">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="174aa-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="174aa-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="174aa-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="174aa-136">ResponseCode</span></span>](responsecode.md)
    
## <a name="updateinboxrules-set-rule-request-example"></a><span data-ttu-id="174aa-137">Exemplo de solicitação UpdateInboxRules (set rule)</span><span class="sxs-lookup"><span data-stu-id="174aa-137">UpdateInboxRules (Set Rule) request example</span></span>

<span data-ttu-id="174aa-138">Você pode usar os serviços Web do Exchange para modificar uma regra de caixa de entrada na caixa de correio de um usuário no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="174aa-138">You can use Exchange Web Services to modify an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="174aa-139">Use o elemento [UpdateInboxRules](updateinboxrules.md) em conjunto com o elemento [SetRuleOperation](setruleoperation.md) para modificar uma regra.</span><span class="sxs-lookup"><span data-stu-id="174aa-139">Use the [UpdateInboxRules](updateinboxrules.md) element in conjunction with the [SetRuleOperation](setruleoperation.md) element to modify a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="174aa-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="174aa-140">Description</span></span>

<span data-ttu-id="174aa-141">O cliente cria a solicitação XML e a envia para o servidor.</span><span class="sxs-lookup"><span data-stu-id="174aa-141">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="174aa-142">Código</span><span class="sxs-lookup"><span data-stu-id="174aa-142">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <Operations xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
          <SetRuleOperation xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="174aa-143">Comentários</span><span class="sxs-lookup"><span data-stu-id="174aa-143">Comments</span></span>

<span data-ttu-id="174aa-144">Este exemplo altera o nome de exibição para "(modificado) isso é lixo eletrônico".</span><span class="sxs-lookup"><span data-stu-id="174aa-144">This example changes the display name to "(Modified) This is Junk".</span></span>
  
> [!NOTE]
> <span data-ttu-id="174aa-145">Os valores dos atributos **ID** e **ChangeKey** do elemento [FolderId](folderid.md) foram reduzidos para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="174aa-145">The values of the **Id** and **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="174aa-146">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="174aa-146">Request elements</span></span>

<span data-ttu-id="174aa-147">A solicitação **UpdateInboxRules** inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="174aa-147">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="174aa-148">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="174aa-148">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="174aa-149">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="174aa-149">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="174aa-150">Operations</span><span class="sxs-lookup"><span data-stu-id="174aa-150">Operations</span></span>](operations.md)
    
<span data-ttu-id="174aa-151">O elemento [Operations](operations.md) contém o elemento [SetRuleOperation](setruleoperation.md) para modificar uma regra.</span><span class="sxs-lookup"><span data-stu-id="174aa-151">The [Operations](operations.md) element contains the [SetRuleOperation](setruleoperation.md) element to modify a rule.</span></span> 
  
## <a name="updateinboxrules-set-rule-response-example"></a><span data-ttu-id="174aa-152">Exemplo de resposta UpdateInboxRules (set rule)</span><span class="sxs-lookup"><span data-stu-id="174aa-152">UpdateInboxRules (Set Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="174aa-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="174aa-153">Description</span></span>

<span data-ttu-id="174aa-154">O exemplo a seguir do corpo SOAP (Simple Object Access Protocol) mostra uma resposta bem-sucedida à solicitação **UpdateInboxRules** que modifica uma regra.</span><span class="sxs-lookup"><span data-stu-id="174aa-154">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that modifies a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="174aa-155">Código</span><span class="sxs-lookup"><span data-stu-id="174aa-155">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" 
        Version="Exchange2010_SP1" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
          ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="174aa-156">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="174aa-156">Successful response elements</span></span>

<span data-ttu-id="174aa-157">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="174aa-157">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="174aa-158">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="174aa-158">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="174aa-159">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="174aa-159">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="174aa-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="174aa-160">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="174aa-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="174aa-161">ResponseCode</span></span>](responsecode.md)
    
## <a name="updateinboxrules-delete-rule-request-example"></a><span data-ttu-id="174aa-162">Exemplo de solicitação UpdateInboxRules (excluir regra)</span><span class="sxs-lookup"><span data-stu-id="174aa-162">UpdateInboxRules (Delete Rule) request example</span></span>

<span data-ttu-id="174aa-163">Você pode usar os serviços Web do Exchange para excluir uma regra de caixa de entrada na caixa de correio de um usuário no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="174aa-163">You can use Exchange Web Services to delete an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="174aa-164">Use o [UpdateInboxRules](updateinboxrules.md) em conjunto com o elemento [DeleteRuleOperation](deleteruleoperation.md) para excluir uma regra.</span><span class="sxs-lookup"><span data-stu-id="174aa-164">Use the [UpdateInboxRules](updateinboxrules.md) in conjunction with the [DeleteRuleOperation](deleteruleoperation.md) element to delete a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="174aa-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="174aa-165">Description</span></span>

<span data-ttu-id="174aa-166">O cliente cria a solicitação XML e a envia para o servidor.</span><span class="sxs-lookup"><span data-stu-id="174aa-166">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="174aa-167">Código</span><span class="sxs-lookup"><span data-stu-id="174aa-167">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="174aa-168">Comentários</span><span class="sxs-lookup"><span data-stu-id="174aa-168">Comments</span></span>

<span data-ttu-id="174aa-169">Este exemplo exclui a regra identificada existente.</span><span class="sxs-lookup"><span data-stu-id="174aa-169">This example deletes the existing identified rule.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="174aa-170">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="174aa-170">Request elements</span></span>

<span data-ttu-id="174aa-171">A solicitação **UpdateInboxRules** inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="174aa-171">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="174aa-172">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="174aa-172">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="174aa-173">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="174aa-173">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="174aa-174">Operations</span><span class="sxs-lookup"><span data-stu-id="174aa-174">Operations</span></span>](operations.md)
    
<span data-ttu-id="174aa-175">O elemento [Operations](operations.md) contém o elemento [DeleteRuleOperation](deleteruleoperation.md) para excluir uma regra.</span><span class="sxs-lookup"><span data-stu-id="174aa-175">The [Operations](operations.md) element contains the [DeleteRuleOperation](deleteruleoperation.md) element to delete a rule.</span></span> 
  
## <a name="updateinboxrules-delete-rule-response-example"></a><span data-ttu-id="174aa-176">Exemplo de resposta UpdateInboxRules (excluir regra)</span><span class="sxs-lookup"><span data-stu-id="174aa-176">UpdateInboxRules (Delete Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="174aa-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="174aa-177">Description</span></span>

<span data-ttu-id="174aa-178">O exemplo a seguir do corpo SOAP (Simple Object Access Protocol) mostra uma resposta bem-sucedida à solicitação **UpdateInboxRules** que exclui uma regra.</span><span class="sxs-lookup"><span data-stu-id="174aa-178">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that deletes a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="174aa-179">Código</span><span class="sxs-lookup"><span data-stu-id="174aa-179">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" 
        Version="Exchange2010_SP1" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="174aa-180">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="174aa-180">Successful response elements</span></span>

<span data-ttu-id="174aa-181">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="174aa-181">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="174aa-182">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="174aa-182">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="174aa-183">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="174aa-183">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="174aa-184">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="174aa-184">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="174aa-185">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="174aa-185">ResponseCode</span></span>](responsecode.md)
    
## <a name="see-also"></a><span data-ttu-id="174aa-186">Confira também</span><span class="sxs-lookup"><span data-stu-id="174aa-186">See also</span></span>



[<span data-ttu-id="174aa-187">Operação GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="174aa-187">GetInboxRules operation</span></span>](getinboxrules-operation.md)

