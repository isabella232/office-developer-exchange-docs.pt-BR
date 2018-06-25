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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837903"
---
# <a name="updateinboxrules-operation"></a>Operação UpdateInboxRules

A operação UpdateInboxRules atualiza regras de caixa de entrada do usuário autenticado, aplicando as operações especificadas. **UpdateInboxRules** é usado para criar uma regra de caixa de entrada, para definir uma regra de caixa de correio ou para excluir uma regra de caixa de entrada. 
  
Quando você usar a operação **UpdateInboxRules** , serviços Web do Exchange exclui regras de envio do lado do cliente. Regras de envio do lado do cliente são armazenadas no cliente na regra de mensagem de informações de associado de pasta (FAI) e em nenhum outro lugar. EWS exclui essa regra mensagem FAI por padrão, com base na expectativa de que o Outlook irá recriá-lo. No entanto, Outlook não puder recriar as regras que não existem também como uma regra estendida e regras de envio do lado do cliente não existirem como regras estendidas. Como resultado, essas regras são perdidas. Sugerimos que você considere o seguinte ao projetar sua solução. 
  
## <a name="updateinboxrules-create-rule-request-example"></a>Exemplo de solicitação de UpdateInboxRules (Criar regra)

Você pode usar os serviços Web do Exchange para criar uma regra de caixa de entrada na caixa de correio do usuário no armazenamento do Exchange. Use o elemento [UpdateInboxRules](updateinboxrules.md) em conjunto com o elemento [CreateRuleOperation](createruleoperation.md) para criar uma regra. 
  
### <a name="description"></a>Descrição

O cliente constrói solicitação XML e o envia ao servidor.
  
### <a name="code"></a>Código

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

### <a name="comments"></a>Comments

Este exemplo cria uma regra que moverá uma mensagem de email para a pasta Lixo eletrônico, se o assunto do email contém uma cadeia de caracteres que é igual a "Interessante".
  
### <a name="request-elements"></a>Elementos de solicitação

A solicitação de **UpdateInboxRules** inclui os seguintes elementos: 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
O elemento de [operações](operations.md) contém o elemento [CreateRuleOperation](createruleoperation.md) para criar uma regra. 
  
## <a name="updateinboxrules-create-rule-response-example"></a>Exemplo de resposta UpdateInboxRules (Criar regra)

### <a name="description"></a>Descrição

O exemplo de corpo simples (SOAP Object Access Protocol) a seguir mostra uma resposta bem-sucedida à solicitação de **UpdateInboxRules** que cria uma regra. 
  
### <a name="code"></a>Código

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

### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedida

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="updateinboxrules-set-rule-request-example"></a>Exemplo de solicitação de UpdateInboxRules (regra definido)

Você pode usar os serviços Web do Exchange para modificar uma regra de caixa de entrada na caixa de correio do usuário no armazenamento do Exchange. Use o elemento [UpdateInboxRules](updateinboxrules.md) em conjunto com o elemento [SetRuleOperation](setruleoperation.md) para modificar uma regra. 
  
### <a name="description"></a>Descrição

O cliente constrói solicitação XML e o envia ao servidor.
  
### <a name="code"></a>Código

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

### <a name="comments"></a>Comments

Este exemplo altera o nome para exibição "(modificado) Esta é lixo".
  
> [!NOTE]
> Os valores de **Id** e **ChangeKey** atributos do elemento [FolderId](folderid.md) foram diminuídos para melhorar a legibilidade. 
  
### <a name="request-elements"></a>Elementos de solicitação

A solicitação de **UpdateInboxRules** inclui os seguintes elementos: 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
O elemento de [operações](operations.md) contém o elemento [SetRuleOperation](setruleoperation.md) para modificar uma regra. 
  
## <a name="updateinboxrules-set-rule-response-example"></a>Exemplo de resposta UpdateInboxRules (regra definido)

### <a name="description"></a>Descrição

O exemplo de corpo simples (SOAP Object Access Protocol) a seguir mostra uma resposta bem-sucedida à solicitação de **UpdateInboxRules** que modifica uma regra. 
  
### <a name="code"></a>Código

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

### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedida

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="updateinboxrules-delete-rule-request-example"></a>Exemplo de solicitação de UpdateInboxRules (Excluir regra)

Você pode usar os serviços Web do Exchange para excluir uma regra de caixa de entrada na caixa de correio do usuário no armazenamento do Exchange. Use o [UpdateInboxRules](updateinboxrules.md) em conjunto com o elemento [DeleteRuleOperation](deleteruleoperation.md) para excluir uma regra. 
  
### <a name="description"></a>Descrição

O cliente constrói solicitação XML e o envia ao servidor.
  
### <a name="code"></a>Código

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

### <a name="comments"></a>Comments

Este exemplo exclui a regra identificada existente.
  
### <a name="request-elements"></a>Elementos de solicitação

A solicitação de **UpdateInboxRules** inclui os seguintes elementos: 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
O elemento de [operações](operations.md) contém o elemento [DeleteRuleOperation](deleteruleoperation.md) para excluir uma regra. 
  
## <a name="updateinboxrules-delete-rule-response-example"></a>Exemplo de resposta UpdateInboxRules (Excluir regra)

### <a name="description"></a>Descrição

O exemplo de corpo simples (SOAP Object Access Protocol) a seguir mostra uma resposta bem-sucedida à solicitação de **UpdateInboxRules** que exclui uma regra. 
  
### <a name="code"></a>Código

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

### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedida

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="see-also"></a>Confira também



[Operação GetInboxRules](getinboxrules-operation.md)

