---
title: Operação RemoveContactFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 28ec96c3-45af-48ff-9f17-718a527dc0ad
description: Encontre informações sobre a operação do EWS do RemoveContactFromImList.
ms.openlocfilehash: 8b3d83a0b53bad169d9f3478540e5087901f3a12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458464"
---
# <a name="removecontactfromimlist-operation"></a>Operação RemoveContactFromImList

Encontre informações sobre a operação do EWS do **RemoveContactFromImList** . 
  
A operação **RemoveContactFromImList** remove contatos da lista de IM (mensagens instantâneas) do Lync quando o Lync usa o Exchange para o repositório de contatos. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-removecontactfromimlist-operation"></a>Usando a operação RemoveContactFromImList

A operação **RemoveContactFromImList** aceita um único argumento que identifica um contato a ser removido da lista de contatos do Lync armazenado em um servidor Exchange. A lista de contatos que esta operação direciona é chamada **contatos do Lync** no Outlook 2013. 
  
> [!CAUTION]
> Não use a [Operação DeleteItem](deleteitem-operation.md) para remover contatos de uma lista de contatos. É possível que o processamento adicional no servidor tenha que ocorrer para dar suporte à remoção de um contato da lista de **contatos do Lync** . Observe que a lista de **contatos do Lync** é o equivalente conceitual da pasta de caixa de correio padrão do **Lync Contacts** . 
  
### <a name="removecontactfromimlist-operation-soap-headers"></a>Cabeçalhos SOAP de operação RemoveContactFromImList

A operação **RemoveContactFromImList** pode usar os cabeçalhos SOAP listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Este cabeçalho é aplicável a uma resposta.  <br/> |
   
## <a name="removecontactfromimlist-operation-request-example-remove-a-contact-from-the-lync-contacts-list"></a>Exemplo de solicitação de operação RemoveContactFromImList: remover um contato da lista de contatos do Lync

O exemplo a seguir de uma solicitação de operação do **RemoveContactFromImList** mostra como remover um contato da lista de **contatos do Lync** . A operação **RemoveContactFromImList** aceita um único identificador de contato exclusivo para identificar o contato removido da lista de **contatos do Lync** . 
  
> [!NOTE]
> Todos os identificadores de item e as chaves de alteração deste artigo foram reduzidos para preservar a legibilidade. 
  
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

Os seguintes elementos são usados na solicitação de corpo SOAP:
  
- [RemoveContactFromImList](removecontactfromimlist.md)
    
- [ContactID](contactid.md)
    
## <a name="successful-removecontactfromimlist-operation-response"></a>Resposta de operação RemoveContactFromImList bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação do **RemoveContactFromImList** para remover um contato da lista de **contatos do Lync** . 
  
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

Os seguintes elementos são usados no corpo SOAP de resposta:
  
- [RemoveContactFromImListResponse](removecontactfromimlistresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="removecontactfromimlist-operation-error-response"></a>Resposta de erro de operação RemoveContactFromImList

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **RemoveContactFromImList** . Esta é uma resposta a uma solicitação para remover um contato da lista de **contatos do Lync** quando o contato não existe mais na lista. 
  
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

Os seguintes elementos são usados no corpo SOAP de resposta de erro:
  
- [RemoveContactFromImListResponse](removecontactfromimlistresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Confira também

- [Operações do EWS no Exchange](ews-operations-in-exchange.md)
    
- [Operação GetImItemList](getimitemlist-operation.md)
    

