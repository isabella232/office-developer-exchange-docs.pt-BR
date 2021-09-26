---
title: Operação GetInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetInboxRules
api_type:
- schema
ms.assetid: b4b2701a-4a23-4acc-8c75-19f7955ad7ae
description: A operação GetInboxRules usa Exchange Web Services para recuperar regras de Caixa de Entrada na caixa de correio do usuário identificado.
ms.openlocfilehash: 3e312ed08494b92c212595d081454b5f2ca6117e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546249"
---
# <a name="getinboxrules-operation"></a>Operação GetInboxRules

A **operação GetInboxRules** usa Exchange Web Services para recuperar regras de Caixa de Entrada na caixa de correio do usuário identificado. 
  
## <a name="getinboxrules-request-example"></a>Exemplo de solicitação GetInboxRules

### <a name="description"></a>Descrição

O exemplo a seguir mostra o XML de solicitação que o cliente envia para o servidor. A solicitação identifica o usuário no elemento [MailboxSmtpAddress.](mailboxsmtpaddress.md) Todas as regras de Caixa de Entrada para o usuário identificado devem ser retornadas na resposta. 
  
### <a name="code"></a>Código

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

### <a name="request-elements"></a>Elementos request

A solicitação inclui o seguinte elemento opcional:
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
## <a name="successful-getinboxrules-response-example"></a>Exemplo de resposta GetInboxRules bem-sucedida

### <a name="description"></a>Descrição

O exemplo de corpo soap (Simple Object Access Protocol) a seguir mostra uma resposta bem-sucedida à **solicitação GetInboxRules.** Neste exemplo, a resposta inclui uma regra. 
  
> [!NOTE]
> Os valores da **Id e** os atributos **ChangeKey** do [elemento FolderId](folderid.md) foram reduzidos para preservar a capacidade de leitura. 
  
### <a name="code"></a>Código

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

### <a name="response-elements"></a>Elementos de resposta

Os seguintes elementos estão incluídos na resposta:
  
- [GetInboxRulesResponse](getinboxrulesresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [OutlookRuleBlobExists](outlookruleblobexists.md)
    
- [InboxRules](inboxrules.md)
    
## <a name="see-also"></a>Confira também



[Operação UpdateInboxRules](updateinboxrules-operation.md)

