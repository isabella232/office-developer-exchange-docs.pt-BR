---
title: Operação GetNonIndexableItemDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a
description: Encontre informações sobre a operação GetNonIndexableItemDetails EWS.
ms.openlocfilehash: d494765d56bc06c2e7f90b99174622b00449116d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516969"
---
# <a name="getnonindexableitemdetails-operation"></a>Operação GetNonIndexableItemDetails

Encontre informações sobre a **operação GetNonIndexableItemDetails** EWS. 
  
A **operação GetNonIndexableItemDetails** recupera detalhes sobre itens que não podem ser indexados. Isso inclui, mas não se limita a, o identificador de item, um código de erro, uma descrição de erro, quando uma tentativa foi feita para indexar o item e informações adicionais sobre o arquivo. 
  
> [!NOTE]
> Embora o esquema indique que mais de uma caixa de correio pode ser pesquisada, na versão de versão inicial do Exchange 2013, o serviço oferece suporte apenas para obter detalhes do item para itens não indexáveis em uma única caixa de correio. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-getnonindexableitemdetails-operation"></a>Usando a operação GetNonIndexableItemDetails

A **operação GetNonIndexableItemDetails** identifica itens de caixa de correio que não podem ser indexados e fornece informações sobre por que os itens não podem ser indexados. Itens que não podem ser indexados não são pesquisados durante uma pesquisa de descoberta. 
  
### <a name="getnonindexableitemdetails-operation-soap-headers"></a>GetNonIndexableItemDetails operation SOAP headers

A **operação GetNonIndexableItemDetails** pode usar os headers SOAP listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |Identifica as funções de servidor necessárias para que o chamador faça a solicitação. Esse header é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Esse header é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Esse header é aplicável a uma resposta.  <br/> |
   
## <a name="getnonindexableitemdetails-operation-request-example-get-the-details-of-an-item-that-cannot-be-indexed"></a>Exemplo da solicitação de operação GetNonIndexableItemDetails: Obter os detalhes de um item que não pode ser indexado

O exemplo a seguir de uma solicitação de operação **GetNonIndexableItemDetails** mostra como solicitar os detalhes de itens que não podem ser indexados para uma única caixa de correio. A pesquisa é realizada em caixas de correio primárias e de arquivo morto. 
  
> [!NOTE]
> Todos os nomes de domínio herdados neste exemplo foram reduzidos para preservar a capacidade de leitura. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetNonIndexableItemDetails>
         <m:Mailboxes>
            <t:LegacyDN>/o=First Organization/ou=Exchange Administrative Group (FYT)/cn=Recipients/cn=35-Steve</t:LegacyDN>
         </m:Mailboxes>
         <m:SearchArchiveOnly>false</m:SearchArchiveOnly>
      </m:GetNonIndexableItemDetails>
   </soap:Body>
</soap:Envelope>

```

O corpo SOAP de solicitação contém os seguintes elementos:
  
- [GetNonIndexableItemDetails](getnonindexableitemdetails.md)
    
- [Mailboxes (NonEmptyArrayOfLegacyDNsType)](mailboxes-nonemptyarrayoflegacydnstype.md)
    
- [LegacyDN](legacydn.md)
    
- [SearchArchiveOnly](searcharchiveonly.md)
    
## <a name="successful-getnonindexableitemdetails-operation-response"></a>Resposta bem-sucedida da operação GetNonIndexableItemDetails

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetNonIndexableItemDetails** para obter itens que não podem ser indexados para uma única caixa de correio. O item neste exemplo que não pode ser indexado é o arquivo binaryfile.abc, que é de um formato desconhecido. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetNonIndexableItemDetailsResponse ResponseClass="Success" 
                                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <NonIndexableItemDetailsResult>
            <Items xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <NonIndexableItemDetail>
                  <ItemId Id="AQMkAGVmNDAyOQAAAY2fUAAAAA==" ChangeKey="CQAAAA=="/>
                  <ErrorCode>DocumentParserFailure</ErrorCode>
                  <ErrorDescription>The document parser encountered a processing error.</ErrorDescription>
                  <IsPartiallyIndexed>false</IsPartiallyIndexed>
                  <IsPermanentFailure>true</IsPermanentFailure>
                  <SortValue>502511175756</SortValue>
                  <AttemptCount>0</AttemptCount>
                  <LastAttemptTime>2012-11-15T01:56:11Z</LastAttemptTime>
                  <AdditionalInfo> 301002 Error parsing document 'exchange://localhost/Attachment/d987b1f4-9aa7-42b3-aa8c-9515a35dfa1a/1f3047d4-c287-41e4-910c-feb70c1a59f0/ef402830-3d33-4a0d-a4e9-d8576900060d/85b83861-0026-418f-8464-be2036696333/502511175756.0/binaryfile.abc'. Document has an undetectable format and will not be parsed.</AdditionalInfo>
               </NonIndexableItemDetail>
            </Items>
         </NonIndexableItemDetailsResult>
      </GetNonIndexableItemDetailsResponse>
   </s:Body>
</s:Envelope>

```

O corpo SOAP de resposta contém os seguintes elementos:
  
- [GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [NonIndexableItemDetailsResult](nonindexableitemdetailsresult.md)
    
- [NonIndexableItemDetail](nonindexableitemdetail.md)
    
- [ItemId](itemid.md)
    
- [ErrorCode (ItemIndexErrorType)](errorcode-itemindexerrortype.md)
    
- [ErrorDescription](errordescription.md)
    
- [IsPartiallyIndexed](ispartiallyindexed.md)
    
- [IsPermanentFailure](ispermanentfailure.md)
    
- [SortValue](sortvalue.md)
    
- [AttemptCount](attemptcount.md)
    
- [LastAttemptTime](lastattempttime.md)
    
- [AdditionalInfo](additionalinfo.md)
    
## <a name="getnonindexableitemdetails-operation-error-response"></a>Resposta de erro da operação GetNonIndexableItemDetails

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetNonIndexableItemDetails.** Esta é uma resposta a uma solicitação para obter detalhes do item para itens que não podem ser indexados de mais de uma caixa de correio. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetNonIndexableItemDetailsResponse ResponseClass="Error" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Multiple mailboxes is currently not supported, only single mailbox is supported.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetNonIndexableItemDetailsResponse>
   </s:Body>
</s:Envelope>
```

O corpo SOAP da resposta de erro contém os seguintes elementos:
  
- [GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Para obter códigos de erro adicionais genéricos para EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Confira também

- [Operações EWS em Exchange](ews-operations-in-exchange.md)
    
- [Operação GetSearchableMailboxes](getsearchablemailboxes-operation.md)
    
- [Operação SearchMailboxes](searchmailboxes-operation.md)
    
- [Operação GetHoldOnMailboxes](getholdonmailboxes-operation.md)
    
- [Operação SetHoldOnMailboxes](setholdonmailboxes-operation.md)
    
- [Operação GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md)
    
- [Operação GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md)
    

