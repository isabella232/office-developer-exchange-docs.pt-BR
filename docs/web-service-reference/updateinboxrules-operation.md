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
# <a name="updateinboxrules-operation"></a>Operação UpdateInboxRules

A operação UpdateInboxRules atualiza as regras de caixa de entrada do usuário autenticado aplicando as operações especificadas. **UpdateInboxRules** é usado para criar uma regra de caixa de entrada, para definir uma regra de caixa de entrada, ou para excluir uma regra de caixa de entrada. 
  
Quando você usa a operação **UpdateInboxRules** , os serviços Web do Exchange excluem as regras de envio do lado do cliente. As regras de envio do lado do cliente são armazenadas no cliente na mensagem de FAI (informações associadas à pasta de regras) e em outro lugar. O EWS exclui essa regra FAI mensagem por padrão, com base na expectativa de que o Outlook a recriará. No entanto, o Outlook não pode recriar regras que não existam também como uma regra estendida e as regras de envio do lado do cliente não existem como regras estendidas. Como resultado, essas regras são perdidas. Sugerimos que você considere isso ao criar sua solução. 
  
## <a name="updateinboxrules-create-rule-request-example"></a>Exemplo de solicitação UpdateInboxRules (criar regra)

Você pode usar os serviços Web do Exchange para criar uma regra de caixa de entrada na caixa de correio de um usuário no repositório do Exchange. Use o elemento [UpdateInboxRules](updateinboxrules.md) em conjunto com o elemento [CreateRuleOperation](createruleoperation.md) para criar uma regra. 
  
### <a name="description"></a>Descrição

O cliente cria a solicitação XML e a envia para o servidor.
  
### <a name="code"></a>Código

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

### <a name="comments"></a>Comentários

Este exemplo cria uma regra que moverá uma mensagem de email para a pasta lixo eletrônico, se o assunto do email contiver uma cadeia de caracteres igual a "interessante".
  
### <a name="request-elements"></a>Elementos Request

A solicitação **UpdateInboxRules** inclui os seguintes elementos: 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
O elemento [Operations](operations.md) contém o elemento [CreateRuleOperation](createruleoperation.md) para criar uma regra. 
  
## <a name="updateinboxrules-create-rule-response-example"></a>Exemplo de resposta UpdateInboxRules (Create Rule)

### <a name="description"></a>Descrição

O exemplo a seguir do corpo SOAP (Simple Object Access Protocol) mostra uma resposta bem-sucedida à solicitação **UpdateInboxRules** que cria uma regra. 
  
### <a name="code"></a>Código

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

### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedidos

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="updateinboxrules-set-rule-request-example"></a>Exemplo de solicitação UpdateInboxRules (set rule)

Você pode usar os serviços Web do Exchange para modificar uma regra de caixa de entrada na caixa de correio de um usuário no repositório do Exchange. Use o elemento [UpdateInboxRules](updateinboxrules.md) em conjunto com o elemento [SetRuleOperation](setruleoperation.md) para modificar uma regra. 
  
### <a name="description"></a>Descrição

O cliente cria a solicitação XML e a envia para o servidor.
  
### <a name="code"></a>Código

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

### <a name="comments"></a>Comentários

Este exemplo altera o nome de exibição para "(modificado) isso é lixo eletrônico".
  
> [!NOTE]
> Os valores dos atributos **ID** e **ChangeKey** do elemento [FolderId](folderid.md) foram reduzidos para legibilidade. 
  
### <a name="request-elements"></a>Elementos Request

A solicitação **UpdateInboxRules** inclui os seguintes elementos: 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
O elemento [Operations](operations.md) contém o elemento [SetRuleOperation](setruleoperation.md) para modificar uma regra. 
  
## <a name="updateinboxrules-set-rule-response-example"></a>Exemplo de resposta UpdateInboxRules (set rule)

### <a name="description"></a>Descrição

O exemplo a seguir do corpo SOAP (Simple Object Access Protocol) mostra uma resposta bem-sucedida à solicitação **UpdateInboxRules** que modifica uma regra. 
  
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

### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedidos

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="updateinboxrules-delete-rule-request-example"></a>Exemplo de solicitação UpdateInboxRules (excluir regra)

Você pode usar os serviços Web do Exchange para excluir uma regra de caixa de entrada na caixa de correio de um usuário no repositório do Exchange. Use o [UpdateInboxRules](updateinboxrules.md) em conjunto com o elemento [DeleteRuleOperation](deleteruleoperation.md) para excluir uma regra. 
  
### <a name="description"></a>Descrição

O cliente cria a solicitação XML e a envia para o servidor.
  
### <a name="code"></a>Código

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

### <a name="comments"></a>Comentários

Este exemplo exclui a regra identificada existente.
  
### <a name="request-elements"></a>Elementos Request

A solicitação **UpdateInboxRules** inclui os seguintes elementos: 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
O elemento [Operations](operations.md) contém o elemento [DeleteRuleOperation](deleteruleoperation.md) para excluir uma regra. 
  
## <a name="updateinboxrules-delete-rule-response-example"></a>Exemplo de resposta UpdateInboxRules (excluir regra)

### <a name="description"></a>Descrição

O exemplo a seguir do corpo SOAP (Simple Object Access Protocol) mostra uma resposta bem-sucedida à solicitação **UpdateInboxRules** que exclui uma regra. 
  
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

### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedidos

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="see-also"></a>Confira também



[Operação GetInboxRules](getinboxrules-operation.md)

