---
title: Operação AddDistributionGroupToImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a
description: Encontre informações sobre o EWS AddDistributionGroupToImList operação.
ms.openlocfilehash: 7c562c317890a4cffb9e5844ea41c1096a8595b4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751045"
---
# <a name="adddistributiongrouptoimlist-operation"></a>Operação AddDistributionGroupToImList

Encontre informações sobre a operação de EWS **AddDistributionGroupToImList** . 
  
A operação de serviços Web do Exchange (EWS) **AddDistributionGroupToImList** adiciona um grupo de distribuição para a lista (IM) no repositório de contato de Unificação de mensagens instantâneas. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-adddistributiongrouptoimlist-operation"></a>Usando a operação AddDistributionGroupToImList

A operação **AddDistributionGroupToImList** aceita um argumento único que identifica um grupo de distribuição para adicionar à lista de mensagens Instantâneas. Esta operação não cria um grupo de distribuição; o grupo de distribuição já deve ser criado. 
  
Esta operação pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.
  
**Tabela 1. Cabeçalhos SOAP AddDistributionGroupToImList operação**

|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Isso é aplicável a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio. Isso é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Isso é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Isso é aplicável a uma resposta.  <br/> |
   
## <a name="adddistributiongrouptoimlist-operation-request-example"></a>Exemplo de solicitação de operação AddDistributionGroupToImList

O exemplo a seguir de uma solicitação de operação **AddDistributionGroupToImList** mostra como adicionar um grupo de distribuição à lista de mensagens Instantâneas. 
  
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
      <m:AddDistributionGroupToImList>
         <m:SmtpAddress>distributionlist1@example.com</m:SmtpAddress>
      </m:AddDistributionGroupToImList>
   </soap:Body>
</soap:Envelope>
```

A solicitação de corpo SOAP contém os seguintes elementos:
  
- [AddDistributionGroupToImList](adddistributiongrouptoimlist.md)   
- [SmtpAddress](smtpaddress.md)
    
## <a name="successful-adddistributiongrouptoimlist-operation-response"></a>Resposta de operação AddDistributionGroupToImList bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **AddDistributionGroupToImList** . 
  
A resposta bem-sucedida contém o nome de exibição do grupo de distribuição, a classe de repositório do Exchange para o grupo de distribuição e o identificador do EWS do novo grupo de distribuição.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"
            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
            xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <s:Header>
      <t:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013"/>
   </s:Header>
   <s:Body>
      <m:AddDistributionGroupToImListResponse ResponseClass="Success">
         <m:ResponseCode>NoError</m:ResponseCode>
         <m:ImGroup>
            <t:DisplayName>distributionlist1@example.com</t:DisplayName>
            <t:GroupType>IPM.DistList.MOC.DG</t:GroupType>
            <t:ExchangeStoreId Id="AAMkAGQ1MjJjAA=" 
                             ChangeKey="EgAAAA=="/>
      </m:ImGroup>
      </m:AddDistributionGroupToImListResponse>
   </s:Body>
</s:Envelope>
```

A resposta SOAP body contém os seguintes elementos:
  
- [AddDistributionGroupToImListResponse](adddistributiongrouptoimlistresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [ImGroup](imgroup.md)
    
- [DisplayName (string)](displayname-string.md)
    
- [GroupType](grouptype.md)
    
- [ExchangeStoreId](exchangestoreid.md)
    
## <a name="adddistributiongrouptoimlist-operation-errorinvalidimdistributiongroupsmtpaddress-error-response"></a>Operação AddDistributionGroupToImList ErrorInvalidImDistributionGroupSmtpAddress resposta de erro

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **AddDistributionGroupToImList** . A seguinte resposta de erro ocorre quando é feita uma tentativa para adicionar um grupo de distribuição que não existe no armazenamento do Exchange. 
  
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
      <AddDistributionGroupToImListResponse ResponseClass="Error" 
                                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified IM distribution group SMTP address is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImDistributionGroupSmtpAddress</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddDistributionGroupToImListResponse>
   </s:Body>
</s:Envelope>
```

A resposta de erro corpo SOAP contém os seguintes elementos:
  
- [AddDistributionGroupToImListResponse](adddistributiongrouptoimlistresponse.md)
    
- [MessageText](messagetext.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Confira também

- [Pessoas e contatos no EWS no Exchange](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)   
- [AddImGroup](addimgroup-operation.md)   
- [RemoveImGroup](removeimgroup-operation.md)
    

