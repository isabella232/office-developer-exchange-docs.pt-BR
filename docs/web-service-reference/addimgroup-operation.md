---
title: Operação AddImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6df6e504-b7c8-4773-b10f-ffa5defac229
description: Encontre informações sobre a operação do EWS do AddImGroup.
ms.openlocfilehash: 38ed12a741d46fe998dc0079ed13973ce9edf5ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462812"
---
# <a name="addimgroup-operation"></a>Operação AddImGroup

Encontre informações sobre a operação do EWS do **AddImGroup** . 
  
A operação do **AddImGroup** do serviços Web do Exchange (EWS) adiciona um novo grupo de mensagens instantâneas (IM) a uma caixa de correio. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-addimgroup-operation"></a>Usando a operação AddImGroup

A operação **AddImGroup** usa apenas um único argumento de nome de exibição. 
  
Essa operação retorna o nome de exibição, o tipo de grupo e o identificador de repositório do Exchange do novo grupo.
  
A operação **AddImGroup** pode usar os cabeçalhos SOAP listados na tabela a seguir. 
  
**Tabela 1. Cabeçalhos SOAP de operação AddImGroup**

|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Isso se aplica a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio. Isso se aplica a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Isso se aplica a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Isso se aplica a uma resposta.  <br/> |
   
## <a name="addimgroup-operation-request-example-create-a-new-im-group"></a>Exemplo de solicitação de operação AddImGroup: criar um novo grupo de IM

O exemplo a seguir de uma solicitação de operação **AddImGroup** mostra como criar um grupo de mensagens instantâneas chamado mycustomerobject. 
  
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
      <m:AddImGroup>
         <m:DisplayName>MyCustomGroup</m:DisplayName>
      </m:AddImGroup>
   </soap:Body>
</soap:Envelope>
```

O corpo SOAP de solicitação contém os seguintes elementos:
  
- [AddImGroup](addimgroup.md)
    
- [DisplayName (cadeia de caracteres)](displayname-string.md)
    
## <a name="successful-addimgroup-operation-response"></a>Resposta de operação AddImGroup bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **AddImGroup** . 
  
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
      <AddImGroupResponse ResponseClass="Success"
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImGroup>
            <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">MyCustomGroup</DisplayName>
            <GroupType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">IPM.DistList.MOC.UserGroup</GroupType>
            <ExchangeStoreId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MAAA="
                             ChangeKey="EgAAAA=="
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/types"/>
         </ImGroup>
      </AddImGroupResponse>
   </s:Body>
</s:Envelope>
```

O corpo SOAP de resposta contém os seguintes elementos:
  
- [AddImGroupResponse](addimgroupresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [Imgroup](imgroup.md)
    
- [DisplayName (cadeia de caracteres)](displayname-string.md)
    
- [GroupType](grouptype.md)
    
- [ExchangeStoreId](exchangestoreid.md)
    
## <a name="addimgroup-operation-error-response"></a>Resposta de erro de operação AddImGroup

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **AddImGroup** . Esta é uma resposta a uma solicitação que contém um caractere que não pode ser usado em um nome de exibição. Observe que esta é uma falha SOAP e não uma mensagem de erro baseada em esquema. O nome de exibição enviado na solicitação é ~! @ # $% ^ &amp; e o erro ocorre no &amp; caractere. O &amp; caractere ocorreu na linha 11 e no caractere 33rd na carga de solicitação. A resposta foi retornada com um código HTTP 500. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="https://schemas.microsoft.com/exchange/services/2006/types">a:ErrorSchemaValidation</faultcode>
         <faultstring xml:lang="en-US">The request failed schema validation: An error occurred while parsing EntityName. Line 11, position 33.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
            <e:Message xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">The request failed schema validation.</e:Message>
            <t:MessageXml xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
               <t:LineNumber>11</t:LineNumber>
               <t:LinePosition>33</t:LinePosition>
               <t:Violation>An error occurred while parsing EntityName. Line 11, position 33.</t:Violation>
            </t:MessageXml>
         </detail>
      </s:Fault>
   </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>Também consulte

- [Pessoas e contatos no EWS no Exchange](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [Operação RemoveImGroup](removeimgroup-operation.md)
    
- [SetImGroup](setimgroup.md)
    

