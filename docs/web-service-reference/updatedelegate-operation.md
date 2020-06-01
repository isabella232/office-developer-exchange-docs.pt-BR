---
title: Operação UpdateDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateDelegate
api_type:
- schema
ms.assetid: 03f618ac-ad1a-4772-9b81-c5bb0f12d6ab
description: A operação UpdateDelegate atualiza as permissões de representante na caixa de correio de uma entidade de segurança.
ms.openlocfilehash: b7cf5325d925f8d6588115a8657a2077e940f9d2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468555"
---
# <a name="updatedelegate-operation"></a>Operação UpdateDelegate

A operação **UpdateDelegate** atualiza as permissões de representante na caixa de correio de uma entidade de segurança. 
  
## <a name="soap-headers"></a>Cabeçalhos SOAP

A operação **UpdateDelegate** pode usar os cabeçalhos SOAP listados e descritos na tabela a seguir. 
  
|**Header**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|Representação  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando.  <br/> |
|MailboxCulture  <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura RFC3066 a ser usada para acessar a caixa de correio.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação.  <br/> |
   
## <a name="updatedelegate-request-example"></a>Exemplo de solicitação UpdateDelegate

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação **UpdateDelegate** mostra como atualizar as permissões de representante na conta user1's. Usuário2 recebe o nível de permissão nenhum para a pasta tarefas e recebe permissão para exibir itens particulares. Usuário3 recebe permissões de revisor para a pasta de diário. As solicitações de reunião são enviadas para os representantes e as informações sobre a solicitação são enviadas para Usuário1. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <UpdateDelegate xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
        <t:EmailAddress>user1@example.com</t:EmailAddress>
      </Mailbox>
      <DelegateUsers>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>user2@example.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:TasksFolderPermissionLevel>None</t:TasksFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ViewPrivateItems>true</t:ViewPrivateItems>
        </t:DelegateUser>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>user3@example.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:JournalFolderPermissionLevel>Reviewer</t:JournalFolderPermissionLevel>
          </t:DelegatePermissions>
        </t:DelegateUser>
      </DelegateUsers>
      <DeliverMeetingRequests>DelegatesAndSendInformationToMe</DeliverMeetingRequests>
    </UpdateDelegate>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

A solicitação [UpdateDelegate](updatedelegate.md) não exige que as atualizações sejam aplicadas aos representantes. Os clientes podem alterar somente a configuração **DeliverMeetingMessage** . 
  
## <a name="updatedelegate-response-example"></a>Exemplo de resposta UpdateDelegate

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida a uma operação **UpdateDelegate** . 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8"
                         MinorVersion="1"
                         MajorBuildNumber="206"
                         MinorBuildNumber="0"
                         Version="Exchange2007_SP1"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:UpdateDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                              ResponseClass="Success"
                              xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1333220396-2200287332-232816053-1117</t:SID>
              <t:PrimarySmtpAddress>User2@example.com</t:PrimarySmtpAddress>
              <t:DisplayName>User2</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>true</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>true</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1333220396-2200287332-232816053-1118</t:SID>
              <t:PrimarySmtpAddress>User3@example.com</t:PrimarySmtpAddress>
              <t:DisplayName>User3</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>true</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:UpdateDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="updatedelegate-error-response-example"></a>Exemplo de resposta de erro UpdateDelegate

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro a uma solicitação **UpdateDelegate** . O erro foi gerado porque o representante não existe na lista de representantes da entidade de segurança. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" 
                         MinorVersion="1" 
                         MajorBuildNumber="206" 
                         MinorBuildNumber="0" 
                         Version="Exchange2007_SP1" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:UpdateDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              ResponseClass="Success" 
                              xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Error">
          <m:MessageText>The user is not a delegate for the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorNotDelegate</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
      </m:UpdateDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Também consulte



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

