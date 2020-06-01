---
title: Operação GetInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetInboxRules
api_type:
- schema
ms.assetid: b4b2701a-4a23-4acc-8c75-19f7955ad7ae
description: A operação GetInboxRules usa os serviços Web do Exchange para recuperar regras de caixa de entrada na caixa de correio do usuário identificado.
ms.openlocfilehash: f4c4c03f55c9f32be4a067024f4387888edd5fe9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457932"
---
# <a name="getinboxrules-operation"></a><span data-ttu-id="a6237-103">Operação GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="a6237-103">GetInboxRules operation</span></span>

<span data-ttu-id="a6237-104">A operação **GetInboxRules** usa os serviços Web do Exchange para recuperar regras de caixa de entrada na caixa de correio do usuário identificado.</span><span class="sxs-lookup"><span data-stu-id="a6237-104">The **GetInboxRules** operation uses Exchange Web Services to retrieve Inbox rules in the identified user's mailbox.</span></span> 
  
## <a name="getinboxrules-request-example"></a><span data-ttu-id="a6237-105">Exemplo de solicitação GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="a6237-105">GetInboxRules request example</span></span>

### <a name="description"></a><span data-ttu-id="a6237-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6237-106">Description</span></span>

<span data-ttu-id="a6237-107">O exemplo a seguir mostra o XML de solicitação que o cliente envia para o servidor.</span><span class="sxs-lookup"><span data-stu-id="a6237-107">The following example shows the request XML that the client sends to the server.</span></span> <span data-ttu-id="a6237-108">A solicitação identifica o usuário no elemento [MailboxSmtpAddress](mailboxsmtpaddress.md) .</span><span class="sxs-lookup"><span data-stu-id="a6237-108">The request identifies the user in the [MailboxSmtpAddress](mailboxsmtpaddress.md) element.</span></span> <span data-ttu-id="a6237-109">Todas as regras de caixa de entrada do usuário identificado serão retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="a6237-109">All Inbox rules for the identified user are to be returned in the response.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a6237-110">Código</span><span class="sxs-lookup"><span data-stu-id="a6237-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetInboxRules>
      <m:MailboxSmtpAddress>User1@Contoso.com</m:MailboxSmtpAddress>
    </m:GetInboxRules>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="a6237-111">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="a6237-111">Request elements</span></span>

<span data-ttu-id="a6237-112">A solicitação inclui o seguinte elemento opcional:</span><span class="sxs-lookup"><span data-stu-id="a6237-112">The request includes the following optional element:</span></span>
  
- [<span data-ttu-id="a6237-113">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="a6237-113">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
## <a name="successful-getinboxrules-response-example"></a><span data-ttu-id="a6237-114">Exemplo de resposta GetInboxRules bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="a6237-114">Successful GetInboxRules response example</span></span>

### <a name="description"></a><span data-ttu-id="a6237-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6237-115">Description</span></span>

<span data-ttu-id="a6237-116">O exemplo a seguir do corpo SOAP (Simple Object Access Protocol) mostra uma resposta bem-sucedida à solicitação **GetInboxRules** .</span><span class="sxs-lookup"><span data-stu-id="a6237-116">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **GetInboxRules** request.</span></span> <span data-ttu-id="a6237-117">Neste exemplo, a resposta inclui uma regra.</span><span class="sxs-lookup"><span data-stu-id="a6237-117">In this example, the response includes one rule.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="a6237-118">Os valores dos atributos **ID** e **ChangeKey** do elemento [FolderId](folderid.md) foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a6237-118">The values of the **Id** and the **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a6237-119">Código</span><span class="sxs-lookup"><span data-stu-id="a6237-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14"
        MinorVersion="1" MajorBuildNumber="139"
        MinorBuildNumber="0"
        Version="Exchange2010_SP1"
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetInboxRulesResponse ResponseClass="Success"
        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <OutlookRuleBlobExists>true</OutlookRuleBlobExists>
      <InboxRules>
        <Rule xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <RuleId>dCsAAABjzvA=</RuleId>
          <DisplayName>MoveInterestingToJunk</DisplayName>
          <Priority>1</Priority>
          <IsEnabled>true</IsEnabled>
          <Conditions>
            <ContainsSubjectStrings>
              <String>Interesting</String>
            </ContainsSubjectStrings>
          </Conditions>
          <Actions>
            <MoveToFolder>
              <FolderId ChangeKey="AQAAAA==" Id="AAMkAGYzZjZm" />
            </MoveToFolder>
          </Actions>
        </Rule>
      </InboxRules>
    </GetInboxRulesResponse>
  </s:Body>
</s:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="a6237-120">Elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="a6237-120">Response elements</span></span>

<span data-ttu-id="a6237-121">Os seguintes elementos estão incluídos na resposta:</span><span class="sxs-lookup"><span data-stu-id="a6237-121">The following elements are included in the response:</span></span>
  
- [<span data-ttu-id="a6237-122">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="a6237-122">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md)
    
- [<span data-ttu-id="a6237-123">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a6237-123">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a6237-124">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="a6237-124">OutlookRuleBlobExists</span></span>](outlookruleblobexists.md)
    
- [<span data-ttu-id="a6237-125">InboxRules</span><span class="sxs-lookup"><span data-stu-id="a6237-125">InboxRules</span></span>](inboxrules.md)
    
## <a name="see-also"></a><span data-ttu-id="a6237-126">Também consulte</span><span class="sxs-lookup"><span data-stu-id="a6237-126">See also</span></span>



[<span data-ttu-id="a6237-127">Operação UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="a6237-127">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)

