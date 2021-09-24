---
title: Operação AddImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 376acc42-2684-4596-aca1-82a4a10865c9
description: Encontre informações sobre a operação AddImContactToGroup EWS.
ms.openlocfilehash: 2f3cfa35662251fdcd449876af466bd5c066ec62
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525404"
---
# <a name="addimcontacttogroup-operation"></a>Operação AddImContactToGroup

Encontre informações sobre **a operação AddImContactToGroup** EWS. 
  
A **operação AddImContactToGroup** Exchange Web Services (EWS) adiciona um contato de mensagens instantâneas (IM) existente a um grupo. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-addimcontacttogroup-operation"></a>Usando a operação AddImContactToGroup

A **operação AddImContactToGroup** só pode aceitar contatos de IM. Se você quiser adicionar um novo contato de IM ao Unified Contact Store, use a [operação AddNewImContactToGroup.](addnewimcontacttogroup-operation.md) 
  
A **operação AddImContactToGroup** pode usar os headers SOAP listados na tabela a seguir. 
  
**Tabela 1. Headers soap da operação AddImContactToGroup**

|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Esse header é aplicável a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido na RFC 3066, "Marcas para a Identificação de Idiomas", a ser usada para acessar a caixa de correio. Esse header é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Esse header é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Esse header é aplicável a uma resposta.  <br/> |
   
## <a name="addimcontacttogroup-operation-request-example-add-an-existing-im-contact-to-an-im-group"></a>Exemplo da solicitação de operação AddImContactToGroup: Adicionar um contato de IM existente a um grupo de IM

O exemplo a seguir de uma solicitação de operação **AddImContactToGroup** mostra como adicionar um contato de IM existente a um grupo de IM. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

O corpo SOAP de solicitação contém os seguintes elementos:
  
- [AddImContactToGroup](addimcontacttogroup.md)
    
- [ContactId](contactid.md)
    
- [GroupId](groupid.md)
    
## <a name="successful-addimcontacttogroup-operation-response"></a>Resposta bem-sucedida da operação AddImContactToGroup

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **AddImContactToGroup.** 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddImContactToGroupResponse ResponseClass="Success" 
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </AddImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

O corpo SOAP de resposta contém os seguintes elementos:
  
- [AddImContactToGroupResponse](addimcontacttogroupresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="addimcontacttogroup-operation-errorinvalidimcontactid-error-response"></a>Resposta de erro da operação AddImContactToGroup ErrorInvalidImContactId

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **AddImContactToGroup.** A seguinte resposta de erro ocorre quando uma tentativa é feita para adicionar um contato que não é um contato de IM. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddImContactToGroupResponse ResponseClass="Error" 
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         </AddImContactToGroupResponse>
      </s:Body>
</s:Envelope>
```

O corpo SOAP da resposta de erro contém os seguintes elementos:
  
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
    
- [Pessoas e contatos no EWS no Exchange](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

