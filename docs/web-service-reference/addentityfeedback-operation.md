---
title: Operação AddEntityFeedback
manager: luken
ms.date: 4/18/2016
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00e40197-5794-4268-b937-bd65aa044890
description: A operação AddEntityFeedback retorna informações de erro correspondentes a problemas no servidor.
ms.openlocfilehash: a1027a0a1ee06cf3e83833b1d84c13d77b07c0b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458436"
---
# <a name="addentityfeedback-operation"></a>Operação AddEntityFeedback

A operação **AddEntityFeedback** retorna informações de erro correspondentes a problemas no servidor. 
  
Essa operação depende do tipo de evento que está sendo registrado em log. Um dos eventos mais importantes é **EntityAdded**, que corresponde a uma entidade que está sendo selecionada. Essa operação é em lote, portanto, ela pode ser usada para registrar lotes de entradas em uma única solicitação. 
  
## <a name="findpeople-request-examples"></a>Exemplos de solicitação FindPeople

A operação **AddEntityFeedback** oferece uma maneira de os clientes registrarem detalhes de interação com entidades retornadas pelo serviço. Isso pode ser usado como um sinal para melhorar a relevância por trás das cenas para cada cliente. Por exemplo, os clientes podem usar essa operação para fornecer comentários sobre entidades de pessoas retornadas de **FindPeople**.
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                             xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:AddEntityFeedback>
            <m:EntityFeedbackEntries>
                  <t:EntityFeedbackEntry>
                        <t:ClientEventTimeUTC> 2015-07-05T22:16:18+00:00</t:ClientEventTimeUTC>
                        <t:ClientEventTimeLocal> 2015-07-05T22:16:18+00:00</t:ClientEventTimeLocal>
                        <t:ClientSessionId>00000000-0000-0000-0000-000000000012</t:ClientSessionId>
                        <t:ClientVersion>15.01.0101.01</t:ClientVersion>
                        <t:ClientId>Web</t:ClientId>
                        <t:TransactionId>123456789</t:TransactionId>
                        <t:EventType>EntityAdded</t:EventType>
                        <t:TargetEntityList>["a","b","c"]</t:TargetEntityList>
                        <t:SourceOfEntityAdded></t:SourceOfEntityAdded>
                        <t:JSONPropertyBag></t:JSONPropertyBag>
                  </t:EntityFeedbackEntry>
                  <t:EntityFeedbackEntry>
                  …
                  </t:EntityFeedbackEntry>
            </m:EntityFeedbackEntries>
      </m:AddEntityFeedback>
   </soap:Body>
</soap:Envelope>

```

### <a name="the-request-soap-body-contents"></a>O conteúdo do corpo SOAP de solicitação

A solicitação SOAP contém um único elemento **EntityFeedbackEntries**. Isso, por sua vez, contém uma matriz de objetos **EntityFeedbackEntry** . Cada entrada na matriz pode conter os seguintes elementos. 
  
|**Parâmetros de solicitação**|**Obrigatório**|**Descrição**|**Tipo**|
|:-----|:-----|:-----|:-----|
|**ClientEventTimeUtc** <br/> |Sim  <br/> |A hora UTC em que o evento ocorreu no lado do cliente.  <br/> |DateTime  <br/> |
|**ClientEventTimeLocal** <br/> |Sim  <br/> |A hora local em que o evento ocorreu no lado do cliente.  <br/> |DateTime  <br/> |
|**ClientId** <br/> |Sim  <br/> |Tipo de cliente (por exemplo, Outlook, OWA, etc.).  <br/> |Enumeração ClientIDtype  <br/> |
|**ClientSessionId** <br/> |Sim  <br/> |GUID que identifica a ID da sessão. Gerado no cliente.  <br/> |GUID  <br/> |
|**ClientVersion** <br/> |Sim  <br/> |Versão do cliente (por exemplo, 15.01.0101.000).  <br/> |String  <br/> |
|**EntityAddSource** <br/> |Não  <br/> |Fonte para EntityAded (por exemplo, EntityRelevanceAPI, tipos, coladas).  <br/> |Enumeração EntityAddSource  <br/> |
|**EntrySequenceNumber** <br/> |Sim  <br/> |Um inteiro incremental por sessão de cliente. Usado para detectar a perda de dados.  <br/> |Int  <br/> |
|**EventType** <br/> |Sim  <br/> |Tipo de evento (por exemplo, entidade adicionada, entidade removida).  <br/> |String  <br/> |
|**JSONPropertyBag** <br/> |Não  <br/> |Propriedades adicionais associadas ao evento (blob JSON de pares chave/valor).  <br/> |Blob JSON  <br/> |
|**TargetEntityList** <br/> |Não  <br/> |Lista de entidades associadas ao evento.  <br/> |Cadeia de caracteres JSON  <br/> |
|**TransactionId** <br/> |Não  <br/> |ID (GUID) que correlaciona a ID nos logs de consulta.  <br/> |String  <br/> |
   
### <a name="successful-addentityfeedback-operation-response"></a>Resposta de operação AddEntityFeedback bem-sucedida

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                                MinorVersion="1" 
                                MajorBuildNumber="228" 
                                MinorBuildNumber="0" 
                                Version="V2_49" 
                                xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                                xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" 
                                                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                                              xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                                              xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope> 

```

### <a name="the-response-soap-body-contains-the-following-elements"></a>O corpo SOAP de resposta contém os seguintes elementos

#### <a name="errors"></a>Erros 
  
A API pode registrar um lote de entradas de comentários, registramos tudo o que podemos. Este campo representa o número de entradas de erro que não foram registradas.
    
#### <a name="errordetails"></a>ErrorDetails
  
Os detalhes referentes aos erros acima são separados por `;` .
    
### <a name="currently-supported-values"></a>Valores compatíveis no momento

|**Enumeração ClientIdtype**|
|:-----|
|Desktop  <br/> |
|Exchange  <br/> |
|IMAP4  <br/> |
|Lync  <br/> |
|, MacMail  <br/> |
|MacOutlook  <br/> |
|Mobile  <br/> |
|Outros  <br/> |
|Outlook  <br/> |
|OutlookService  <br/> |
|CORREIO  <br/> |
|Tablet  <br/> |
|Web  <br/> |
   
|**Enumeração EntityAddSource**|
|:-----|
|ActiveDirectory  <br/> |
|EntityRelevanceApi  <br/> |
|EntityRelevanceApiCache  <br/> |
|ExplicitTyping  <br/> |
|LocalCache  <br/> |
|LocalCacheAndEntityRelevanceAPI  <br/> |
|Nenhum  <br/> |
|Outros  <br/> |
|Colar  <br/> |
   
### <a name="addentityfeedback-operation-error-response"></a>Resposta de erro de operação AddEntityFeedback

Para códigos de erro genéricos para EWS, confira [ResponseCode](responsecode.md).
  
### <a name="example-of-addentityfeedback-in-conjunction-with-findpeople"></a>Exemplo de AddEntityFeedback em conjunto com FindPeople

#### <a name="findpeople-request"></a>Solicitação FindPeople
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
<soap:Body >
    <m:FindPeople>
      <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
      <m:QueryString>user1</m:QueryString>
      <m:SearchPeopleSuggestionIndex>true</m:SearchPeopleSuggestionIndex>
    </m:FindPeople>
  </soap:Body>
</soap:Envelope>    
    
```

#### <a name="findpeople-response"></a>Resposta FindPeople

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <FindPeopleResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <People>
                <Persona xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                    <PersonaId Id="AAUQAFjZ4UxX8SZCqSPFsmh0cSo=" />
                    <PersonaType>Person</PersonaType>
                    <CreationTime>2015-10-02T23:25:42</CreationTime>
                    <DisplayName>user2</DisplayName>
…
                  </Persona>
            </People>
            <TotalNumberOfPeopleInView>0</TotalNumberOfPeopleInView>
            <FirstMatchingRowIndex>0</FirstMatchingRowIndex>
            <FirstLoadedRowIndex>0</FirstLoadedRowIndex>
            <TransactionId>b56ad16e-5d5a-4574-90f8-b8dd57382be6</TransactionId>
        </FindPeopleResponse>
    </s:Body>
</s:Envelope>

```

#### <a name="addentityfeedback-request"></a>Solicitação AddEntityFeedback

```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:AddEntityFeedback>
<m:EntityFeedbackEntries>
<t:EntityFeedbackEntry>
         <t:ClientEventTimeUtc>2015-07-05T22:16:18+00:00</t:ClientEventTimeUtc>
         <t:ClientEventTimeLocal>2015-07-05T22:16:18+00:00</t:ClientEventTimeLocal>
         <t:ClientSessionId>00000000-0000-0000-0000-000000000012</t:ClientSessionId>
         <t:ClientVersion>15.01.0101.01</t:ClientVersion>
         <t:ClientId>Web</t:ClientId>
         <t:TransactionId>b56ad16e-5d5a-4574-90f8-b8dd57382be6</t:TransactionId>
         <t:EventType>EntityAdded</t:EventType>
         <t:TargetEntityList>["user1@ms7.com"]</t:TargetEntityList>
         <t:SourceOfEntityAdded>EntityRelevanceApi</t:SourceOfEntityAdded>
         <t:JSONPropertyBag></t:JSONPropertyBag>
</t:EntityFeedbackEntry>
</m:EntityFeedbackEntries>
      </m:AddEntityFeedback>
   </soap:Body>
</soap:Envelope>

```

> [!NOTE]
> Usando a ID de transação de resposta FindPeople como a ID de transação de solicitação AddEntityFeedback. 
  
#### <a name="addentityfeedback-response"></a>Resposta AddEntityFeedback

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope>

```


