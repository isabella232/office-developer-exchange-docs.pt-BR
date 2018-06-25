---
title: Operação AddImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 376acc42-2684-4596-aca1-82a4a10865c9
description: Encontre informações sobre o EWS AddImContactToGroup operação.
ms.openlocfilehash: 669d798b6cabc1cab1fc057a3e18c565467440f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751046"
---
# <a name="addimcontacttogroup-operation"></a>Operação AddImContactToGroup

Encontre informações sobre a operação de EWS **AddImContactToGroup** . 
  
A operação de serviços Web do Exchange (EWS) **AddImContactToGroup** adiciona um contato existente de mensagens instantâneas (IM) a um grupo. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-addimcontacttogroup-operation"></a>Usando a operação AddImContactToGroup

A operação **AddImContactToGroup** só pode aceitar contatos de mensagens Instantâneas. Se você deseja adicionar um novo contato de mensagens Instantâneas para o repositório unificado de contatos, use a operação de [AddNewImContactToGroup](addnewimcontacttogroup-operation.md) . 
  
A operação **AddImContactToGroup** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir. 
  
**Tabela 1. Cabeçalhos SOAP AddImContactToGroup operação**

|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Este cabeçalho é aplicável a uma resposta.  <br/> |
   
## <a name="addimcontacttogroup-operation-request-example-add-an-existing-im-contact-to-an-im-group"></a>Exemplo de solicitação de operação AddImContactToGroup: adicionar um IM existente entre em contato com a um grupo de mensagens Instantâneas

O exemplo a seguir de uma solicitação de operação **AddImContactToGroup** mostra como adicionar um contato de mensagens Instantâneas existente, um grupo de mensagens Instantâneas. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:AddImContactToGroup>
         <m:ContactId Id="AAMkAGQ1MjJjMTBkLTc4Y2AA="
                      ChangeKey="EQAAABYAAABtF8oI7i"/>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkzzAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:AddImContactToGroup>
   </soap:Body>
</soap:Envelope>
```

A solicitação de corpo SOAP contém os seguintes elementos:
  
- [AddImContactToGroup](addimcontacttogroup.md)
    
- [ID de contato](contactid.md)
    
- [GroupId](groupid.md)
    
## <a name="successful-addimcontacttogroup-operation-response"></a>Resposta de operação AddImContactToGroup bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **AddImContactToGroup** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddImContactToGroupResponse ResponseClass="Success" 
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </AddImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

A resposta SOAP body contém os seguintes elementos:
  
- [AddImContactToGroupResponse](addimcontacttogroupresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="addimcontacttogroup-operation-errorinvalidimcontactid-error-response"></a>Operação AddImContactToGroup ErrorInvalidImContactId resposta de erro

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **AddImContactToGroup** . A seguinte resposta de erro ocorre quando é feita uma tentativa para adicionar um contato que não seja um contato de mensagens Instantâneas. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddImContactToGroupResponse ResponseClass="Error" 
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         </AddImContactToGroupResponse>
      </s:Body>
</s:Envelope>
```

A resposta de erro corpo SOAP contém os seguintes elementos:
  
- [AddImContactToGroupResponse](addimcontacttogroupresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Confira também

- [Operação AddImGroup](addimgroup-operation.md)
    
- [Operação AddNewImContactToGroup](addnewimcontacttogroup-operation.md)
    
- [Operação SetImGroup](setimgroup-operation.md)
    
- [Operação RemoveImGroup](removeimgroup-operation.md)
    
- [Operação GetImItemList](getimitemlist-operation.md)
    
- [Pessoas e contatos no EWS no Exchange](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

