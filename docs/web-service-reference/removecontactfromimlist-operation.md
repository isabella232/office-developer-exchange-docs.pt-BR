---
title: Operação RemoveContactFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 28ec96c3-45af-48ff-9f17-718a527dc0ad
description: Encontre informações sobre a operação RemoveContactFromImList EWS.
ms.openlocfilehash: cc72dc1b0abf9032fabafbaac53d29f41968dafb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523583"
---
# <a name="removecontactfromimlist-operation"></a>Operação RemoveContactFromImList

Encontre informações sobre a **operação RemoveContactFromImList** EWS. 
  
A **operação RemoveContactFromImList** remove contatos da lista de mensagens instantâneas (IM) do Lync quando o Lync usa Exchange para o armazenamento de contatos. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-removecontactfromimlist-operation"></a>Usando a operação RemoveContactFromImList

A **operação RemoveContactFromImList** aceita um único argumento que identifica um contato a ser removido da lista de contatos do Lync armazenada em um servidor Exchange. A lista de contatos destinados a essa operação é chamada **de Contatos do Lync** no Outlook 2013. 
  
> [!CAUTION]
> Não use a operação [DeleteItem](deleteitem-operation.md) para remover contatos de uma lista de contatos. O processamento adicional do lado do servidor pode ter que ocorrer para dar suporte à remoção de um contato da lista **contatos do Lync.** Observe que a **lista contatos do Lync** é o equivalente conceitual da pasta de caixa de correio padrão do **Lync Contacts.** 
  
### <a name="removecontactfromimlist-operation-soap-headers"></a>Headers SOAP da operação RemoveContactFromImList

A **operação RemoveContactFromImList** pode usar os headers SOAP listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Esse header é aplicável a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido na RFC 3066, "Marcas para a Identificação de Idiomas", a ser usada para acessar a caixa de correio. Esse header é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Esse header é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Esse header é aplicável a uma resposta.  <br/> |
   
## <a name="removecontactfromimlist-operation-request-example-remove-a-contact-from-the-lync-contacts-list"></a>Exemplo da solicitação de operação RemoveContactFromImList: Remover um contato da lista contatos do Lync

O exemplo a seguir de uma solicitação de operação **RemoveContactFromImList** mostra como remover um contato da lista contatos **do Lync.** A **operação RemoveContactFromImList** aceita um único identificador de contato exclusivo para identificar o contato removido da lista de contatos do **Lync.** 
  
> [!NOTE]
> Todos os identificadores de item e teclas de alteração neste artigo foram reduzidos para preservar a capacidade de leitura. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:RemoveContactFromImList>
         <m:ContactId Id=""/>
      </m:RemoveContactFromImList>
   </soap:Body>
</soap:Envelope>

```

Os seguintes elementos são usados no corpo SOAP da solicitação:
  
- [RemoveContactFromImList](removecontactfromimlist.md)
    
- [ContactId](contactid.md)
    
## <a name="successful-removecontactfromimlist-operation-response"></a>Resposta bem-sucedida da operação RemoveContactFromImList

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **RemoveContactFromImList** para remover um contato da lista contatos **do Lync.** 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Success" 
                                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>
```

Os seguintes elementos são usados no corpo SOAP da resposta:
  
- [RemoveContactFromImListResponse](removecontactfromimlistresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="removecontactfromimlist-operation-error-response"></a>Resposta de erro de operação RemoveContactFromImList

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **RemoveContactFromImList.** Esta é uma resposta a uma solicitação para remover um contato da lista contatos do **Lync** quando o contato não existir mais na lista. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Error" 
                                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>

```

Os seguintes elementos são usados no corpo SOAP da resposta de erro:
  
- [RemoveContactFromImListResponse](removecontactfromimlistresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Confira também

- [Operações EWS em Exchange](ews-operations-in-exchange.md)
    
- [Operação GetImItemList](getimitemlist-operation.md)
    

