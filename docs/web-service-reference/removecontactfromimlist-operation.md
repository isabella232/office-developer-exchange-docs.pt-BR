---
title: Operação RemoveContactFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 28ec96c3-45af-48ff-9f17-718a527dc0ad
description: Encontre informações sobre o EWS RemoveContactFromImList operação.
ms.openlocfilehash: 036b295a84e86ad74c467572cc52fdf6bbae5191
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825080"
---
# <a name="removecontactfromimlist-operation"></a>Operação RemoveContactFromImList

Encontre informações sobre a operação de EWS **RemoveContactFromImList** . 
  
A operação **RemoveContactFromImList** remove contatos da lista de mensagens instantâneas (IM) de Lync quando o Lync usa o Exchange para o armazenamento de contato. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-removecontactfromimlist-operation"></a>Usando a operação RemoveContactFromImList

A operação **RemoveContactFromImList** aceita um argumento único que identifica um contato para remover da lista de contatos Lync armazenada em um servidor Exchange. A lista de contatos que destinos essa operação é chamado de **Contatos do Lync** no Outlook 2013. 
  
> [!CAUTION]
> Não use a [operação DeleteItem](deleteitem-operation.md) para remover contatos de uma lista de contatos. Processamento do lado do servidor adicionais talvez seja necessário ocorrem para oferecer suporte à remoção de um contato da lista de **Contatos do Lync** . Observe que a lista de **Contatos do Lync** é o equivalente conceitual da pasta padrão **Contatos do Lync** da caixa de correio. 
  
### <a name="removecontactfromimlist-operation-soap-headers"></a>Cabeçalhos SOAP RemoveContactFromImList operação

A operação **RemoveContactFromImList** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Este cabeçalho é aplicável a uma resposta.  <br/> |
   
## <a name="removecontactfromimlist-operation-request-example-remove-a-contact-from-the-lync-contacts-list"></a>Exemplo de solicitação de operação RemoveContactFromImList: remover um contato da lista Contatos do Lync

O exemplo a seguir de uma solicitação de operação **RemoveContactFromImList** mostra como remover um contato da lista **Contatos do Lync** . A operação **RemoveContactFromImList** aceita um único identificador exclusivo de contato para identificar o contato que é removido da lista de **Contatos do Lync** . 
  
> [!NOTE]
> Todos os identificadores de itens e teclas de alteração neste artigo foram diminuídas para preservar a legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
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

Os seguintes elementos são usados na solicitação de corpo SOAP:
  
- [RemoveContactFromImList](removecontactfromimlist.md)
    
- [ID de contato](contactid.md)
    
## <a name="successful-removecontactfromimlist-operation-response"></a>Resposta de operação RemoveContactFromImList bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **RemoveContactFromImList** para remover um contato da lista de **Contatos do Lync** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Success" 
                                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>
```

Os seguintes elementos são usados no corpo SOAP de resposta:
  
- [RemoveContactFromImListResponse](removecontactfromimlistresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="removecontactfromimlist-operation-error-response"></a>Resposta de erro de operação RemoveContactFromImList

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **RemoveContactFromImList** . Esta é uma resposta a uma solicitação para remover um contato da lista **Contatos do Lync** , quando o contato não existe mais na lista. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Error" 
                                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>

```

A resposta de erro corpo SOAP são usados os seguintes elementos:
  
- [RemoveContactFromImListResponse](removecontactfromimlistresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Confira também

- [Operações do EWS no Exchange](ews-operations-in-exchange.md)
    
- [Operação GetImItemList](getimitemlist-operation.md)
    

