---
title: Operação UpdateInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateInboxRules
api_type:
- schema
ms.assetid: f982a237-471e-45c5-a2b5-468cfc53150b
description: A operação UpdateInboxRules atualiza as regras de Caixa de Entrada do usuário autenticado aplicando as operações especificadas. UpdateInboxRules é usado para criar uma regra de Caixa de Entrada, para definir uma regra de Caixa de Entrada ou para excluir uma regra de Caixa de Entrada.
ms.openlocfilehash: 08f46219bcb01f5f1c9d69cfaa8b4934e82ff5bd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510712"
---
# <a name="updateinboxrules-operation"></a>Operação UpdateInboxRules

A operação UpdateInboxRules atualiza as regras de Caixa de Entrada do usuário autenticado aplicando as operações especificadas. **UpdateInboxRules** é usado para criar uma regra de Caixa de Entrada, para definir uma regra de Caixa de Entrada ou para excluir uma regra de Caixa de Entrada. 
  
Quando você usa a **operação UpdateInboxRules,** Exchange Web Services exclui regras de envio do lado do cliente. As regras de envio do lado do cliente são armazenadas no cliente na regra FaI (Informações Associadas à Pasta) Mensagem e em nenhum outro lugar. O EWS exclui essa mensagem FAI de regra por padrão, com base na expectativa de que Outlook a recriará. No entanto, Outlook não pode recriar regras que também não existem como uma regra estendida, e as regras de envio do lado do cliente não existem como regras estendidas. Como resultado, essas regras são perdidas. Sugerimos que você considere isso ao projetar sua solução. 
  
## <a name="updateinboxrules-create-rule-request-example"></a>Exemplo de solicitação UpdateInboxRules (Criar Regra)

Você pode usar Exchange Web Services para criar uma regra de Caixa de Entrada na caixa de correio de um usuário no Exchange store. Use o [elemento UpdateInboxRules](updateinboxrules.md) em conjunto com o [elemento CreateRuleOperation](createruleoperation.md) para criar uma regra. 
  
### <a name="description"></a>Descrição

O cliente constrói o XML de solicitação e o envia para o servidor.
  
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

Este exemplo cria uma regra que move uma mensagem de email para a pasta Lixo Eletrônico se o assunto de email contiver uma cadeia de caracteres que seja igual a "Interessante".
  
### <a name="request-elements"></a>Elementos request

A **solicitação UpdateInboxRules** inclui os seguintes elementos: 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
O [elemento Operations](operations.md) contém o elemento [CreateRuleOperation](createruleoperation.md) para criar uma regra. 
  
## <a name="updateinboxrules-create-rule-response-example"></a>Exemplo de resposta UpdateInboxRules (Criar Regra)

### <a name="description"></a>Descrição

O exemplo de corpo soap (Simple Object Access Protocol) a seguir mostra uma resposta bem-sucedida à solicitação **UpdateInboxRules** que cria uma regra. 
  
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
    
## <a name="updateinboxrules-set-rule-request-example"></a>Exemplo de solicitação UpdateInboxRules (Definir Regra)

Você pode usar Exchange Web Services para modificar uma regra de Caixa de Entrada na caixa de correio de um usuário no Exchange store. Use o [elemento UpdateInboxRules](updateinboxrules.md) em conjunto com o [elemento SetRuleOperation](setruleoperation.md) para modificar uma regra. 
  
### <a name="description"></a>Descrição

O cliente constrói o XML de solicitação e o envia para o servidor.
  
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

Este exemplo altera o nome de exibição para "(Modificado) This is Junk".
  
> [!NOTE]
> Os valores dos atributos **Id** e **ChangeKey** do [elemento FolderId](folderid.md) foram reduzidos para a capacidade de leitura. 
  
### <a name="request-elements"></a>Elementos request

A **solicitação UpdateInboxRules** inclui os seguintes elementos: 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
O [elemento Operations](operations.md) contém o elemento [SetRuleOperation](setruleoperation.md) para modificar uma regra. 
  
## <a name="updateinboxrules-set-rule-response-example"></a>Exemplo de resposta UpdateInboxRules (Definir Regra)

### <a name="description"></a>Descrição

O exemplo de corpo soap (Simple Object Access Protocol) a seguir mostra uma resposta bem-sucedida à solicitação **UpdateInboxRules** que modifica uma regra. 
  
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
    
## <a name="updateinboxrules-delete-rule-request-example"></a>Exemplo de solicitação UpdateInboxRules (Excluir Regra)

Você pode usar Exchange Web Services para excluir uma regra de Caixa de Entrada na caixa de correio de um usuário no Exchange store. Use [o UpdateInboxRules](updateinboxrules.md) em conjunto com o [elemento DeleteRuleOperation](deleteruleoperation.md) para excluir uma regra. 
  
### <a name="description"></a>Descrição

O cliente constrói o XML de solicitação e o envia para o servidor.
  
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
  
### <a name="request-elements"></a>Elementos request

A **solicitação UpdateInboxRules** inclui os seguintes elementos: 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
O [elemento Operations](operations.md) contém o elemento [DeleteRuleOperation](deleteruleoperation.md) para excluir uma regra. 
  
## <a name="updateinboxrules-delete-rule-response-example"></a>Exemplo de resposta UpdateInboxRules (Excluir Regra)

### <a name="description"></a>Descrição

O exemplo de corpo soap (Simple Object Access Protocol) a seguir mostra uma resposta bem-sucedida à solicitação **UpdateInboxRules** que exclui uma regra. 
  
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

