---
title: Operação RemoveDistributionGroupFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 252bddf2-98b6-4824-b548-2fba2bda5384
description: Encontre informações sobre a operação do EWS do RemoveDistributionGroupFromImList.
ms.openlocfilehash: 66220f0cab99f404e17136bbb7836ca13d569b53
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459599"
---
# <a name="removedistributiongroupfromimlist-operation"></a>Operação RemoveDistributionGroupFromImList

Encontre informações sobre a operação do EWS do **RemoveDistributionGroupFromImList** . 
  
A operação **RemoveDistributionGroupFromImList** remove um grupo de distribuição da lista de IM (mensagens instantâneas) do Lync quando o Lync usa o Exchange para o repositório de contatos. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-removedistributiongroupfromimlist-operation"></a>Usando a operação RemoveDistributionGroupFromImList

A operação **RemoveDistributionGroupFromImList** aceita um único argumento que identifica um grupo de distribuição a ser removido da lista de mensagens instantâneas do Lync armazenada em um servidor Exchange. 
  
### <a name="removedistributiongroupfromimlist-operation-soap-headers"></a>Cabeçalhos SOAP de operação RemoveDistributionGroupFromImList

A operação **RemoveDistributionGroupFromImList** pode usar os cabeçalhos SOAP listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Este cabeçalho é aplicável a uma resposta.  <br/> |
   
## <a name="removedistributiongroupfromimlist-operation-request-example-remove-a-distribution-group-from-an-im-list"></a>Exemplo de solicitação de operação RemoveDistributionGroupFromImList: remover um grupo de distribuição de uma lista de mensagens instantâneas

O exemplo a seguir de uma solicitação de operação **RemoveDistributionGroupFromImList** mostra como remover um grupo de distribuição de um grupo de mensagens instantâneas. A operação **RemoveDistributionGroupFromImList** aceita o identificador de grupo exclusivo para identificar o grupo de distribuição a ser removido da lista de mensagens instantâneas. O elemento [ExchangeStoreId](exchangestoreid.md) que é retornado na resposta para a [operação GetImItemList](getimitemlist-operation.md) e a [operação AddDistributionGroupToImList](adddistributiongrouptoimlist-operation.md) identifica os grupos de distribuição que podem ser removidos da lista de mensagens instantâneas. 
  
> [!NOTE]
> Todos os identificadores de item e as chaves de alteração deste artigo foram reduzidos para preservar a legibilidade. 
  
```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:RemoveDistributionGroupFromImList>
         <m:GroupId Id="AAMkADEzO4QrAABmEh5oAAA="/>
      </m:RemoveDistributionGroupFromImList>
   </soap:Body>
</soap:Envelope>
```

Os seguintes elementos são usados na solicitação de corpo SOAP:
  
- [RemoveDistributionGroupFromImList](removedistributiongroupfromimlist.md)
    
- [GroupId](groupid.md)
    
## <a name="successful-removedistributiongroupfromimlist-operation-response"></a>Resposta de operação RemoveDistributionGroupFromImList bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **RemoveDistributionGroupFromImList** para um grupo de distribuição de um grupo de mensagens instantâneas. 
  
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
      <RemoveDistributionGroupFromImListResponse ResponseClass="Success" 
                                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveDistributionGroupFromImListResponse>
   </s:Body>
</s:Envelope>
```

Os seguintes elementos são usados no corpo SOAP de resposta:
  
- [RemoveDistributionGroupFromImListResponse](removedistributiongroupfromimlistresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="removedistributiongroupfromimlist-operation-error-response-example"></a>Exemplo de resposta de erro de operação RemoveDistributionGroupFromImList

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **RemoveDistributionGroupFromImList** . Esta é uma resposta a uma solicitação para remover um grupo de distribuição que já foi removido da caixa de correio. 
  
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
      <RemoveDistributionGroupFromImListResponse ResponseClass="Error" 
                                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveDistributionGroupFromImListResponse>
   </s:Body>
</s:Envelope>
```

Os seguintes elementos são usados no corpo SOAP de resposta de erro:
  
- [RemoveDistributionGroupFromImListResponse](removedistributiongroupfromimlistresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Também consulte

- [Operações do EWS no Exchange](ews-operations-in-exchange.md)
    
- [Operação GetImItemList](getimitemlist-operation.md)
    
- [Operação AddDistributionGroupToImList](adddistributiongrouptoimlist-operation.md)
    
- [Pessoas e contatos no EWS no Exchange](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx#What)
    

