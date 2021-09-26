---
title: Operação AddDistributionGroupToImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a
description: Encontre informações sobre a operação AddDistributionGroupToImList EWS.
ms.openlocfilehash: 2dce8e903affb277f40b89859b234828d3ffd941
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546830"
---
# <a name="adddistributiongrouptoimlist-operation"></a>Operação AddDistributionGroupToImList

Encontre informações sobre **a operação AddDistributionGroupToImList** EWS. 
  
A **operação AddDistributionGroupToImList** Exchange Web Services (EWS) adiciona um grupo de distribuição à lista de mensagens instantâneas (IM) no Unified Contact Store. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-adddistributiongrouptoimlist-operation"></a>Usando a operação AddDistributionGroupToImList

A **operação AddDistributionGroupToImList** tem um único argumento que identifica um grupo de distribuição a ser acrescentado à lista de IM. Esta operação não cria um grupo de distribuição; o grupo de distribuição já deve ser criado. 
  
Essa operação pode usar os headers SOAP listados na tabela a seguir.
  
**Tabela 1. Headers SOAP da operação AddDistributionGroupToImList**

|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Isso é aplicável a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido na RFC 3066, "Marcas para a Identificação de Idiomas", a ser usada para acessar a caixa de correio. Isso é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Isso é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Isso é aplicável a uma resposta.  <br/> |
   
## <a name="adddistributiongrouptoimlist-operation-request-example"></a>Exemplo de solicitação de operação AddDistributionGroupToImList

O exemplo a seguir de uma solicitação de operação **AddDistributionGroupToImList** mostra como adicionar um grupo de distribuição à lista de IM. 
  
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
      <m:AddDistributionGroupToImList>
         <m:SmtpAddress>distributionlist1@example.com</m:SmtpAddress>
      </m:AddDistributionGroupToImList>
   </soap:Body>
</soap:Envelope>
```

O corpo SOAP de solicitação contém os seguintes elementos:
  
- [AddDistributionGroupToImList](adddistributiongrouptoimlist.md)   
- [SmtpAddress](smtpaddress.md)
    
## <a name="successful-adddistributiongrouptoimlist-operation-response"></a>Resposta bem-sucedida da operação AddDistributionGroupToImList

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **AddDistributionGroupToImList.** 
  
A resposta bem-sucedida contém o nome de exibição do grupo de distribuição, a classe Exchange de armazenamento do grupo de distribuição e o identificador EWS do novo grupo de distribuição.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"
            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
            xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

O corpo SOAP de resposta contém os seguintes elementos:
  
- [AddDistributionGroupToImListResponse](adddistributiongrouptoimlistresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [ImGroup](imgroup.md)
    
- [DisplayName (cadeia de caracteres)](displayname-string.md)
    
- [GroupType](grouptype.md)
    
- [ExchangeStoreId](exchangestoreid.md)
    
## <a name="adddistributiongrouptoimlist-operation-errorinvalidimdistributiongroupsmtpaddress-error-response"></a>Resposta de erro da operação AddDistributionGroupToImList ErrorInvalidImDistributionGroupSmtpAddress

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **AddDistributionGroupToImList.** A seguinte resposta de erro ocorre quando uma tentativa é feita para adicionar um grupo de distribuição que não existe no Exchange store. 
  
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
      <AddDistributionGroupToImListResponse ResponseClass="Error" 
                                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified IM distribution group SMTP address is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImDistributionGroupSmtpAddress</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddDistributionGroupToImListResponse>
   </s:Body>
</s:Envelope>
```

O corpo SOAP da resposta de erro contém os seguintes elementos:
  
- [AddDistributionGroupToImListResponse](adddistributiongrouptoimlistresponse.md)
    
- [MessageText](messagetext.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Confira também

- [Pessoas e contatos no EWS no Exchange](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)   
- [AddImGroup](addimgroup-operation.md)   
- [RemoveImGroup](removeimgroup-operation.md)
    

