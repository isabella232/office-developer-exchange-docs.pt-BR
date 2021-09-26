---
title: Operação AddImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 6df6e504-b7c8-4773-b10f-ffa5defac229
description: Encontre informações sobre a operação AddImGroup EWS.
ms.openlocfilehash: 9aba6a22502c1006da06ce4a9bc925f13b5b5100
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544357"
---
# <a name="addimgroup-operation"></a>Operação AddImGroup

Encontre informações sobre a **operação AddImGroup** EWS. 
  
A **operação AddImGroup** Exchange Web Services (EWS) adiciona um novo grupo de mensagens instantâneas (IM) a uma caixa de correio. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-addimgroup-operation"></a>Usando a operação AddImGroup

A **operação AddImGroup** só aceita um único argumento de nome de exibição. 
  
Essa operação retorna o nome de exibição, o tipo de grupo e Exchange de armazenamento do novo grupo.
  
A **operação AddImGroup** pode usar os headers SOAP listados na tabela a seguir. 
  
**Tabela 1. Headers SOAP da operação AddImGroup**

|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Isso é aplicável a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido na RFC 3066, "Marcas para a Identificação de Idiomas", a ser usada para acessar a caixa de correio. Isso é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Isso é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Isso é aplicável a uma resposta.  <br/> |
   
## <a name="addimgroup-operation-request-example-create-a-new-im-group"></a>Exemplo da solicitação de operação AddImGroup: Criar um novo grupo de IM

O exemplo a seguir de **uma solicitação de operação AddImGroup** mostra como criar um grupo de IM chamado MyCustomerGroup. 
  
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
    
## <a name="successful-addimgroup-operation-response"></a>Resposta bem-sucedida da operação AddImGroup

O exemplo a seguir mostra uma resposta bem-sucedida a uma **solicitação de operação AddImGroup.** 
  
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
    
- [ImGroup](imgroup.md)
    
- [DisplayName (cadeia de caracteres)](displayname-string.md)
    
- [GroupType](grouptype.md)
    
- [ExchangeStoreId](exchangestoreid.md)
    
## <a name="addimgroup-operation-error-response"></a>Resposta de erro da operação AddImGroup

O exemplo a seguir mostra uma resposta de erro a uma **solicitação de operação AddImGroup.** Esta é uma resposta a uma solicitação que contém um caractere que não pode ser usado em um nome de exibição. Observe que isso é uma falha SOAP e não uma mensagem de erro baseada em esquema. O nome de exibição enviado na solicitação é ~!@#$%^ e o erro &amp; ocorre no &amp; caractere. O &amp; caractere ocorreu na linha 11 e no 33º caractere na carga de solicitação. A resposta foi retornada com um código HTTP 500. 
  
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

## <a name="see-also"></a>Confira também

- [Pessoas e contatos no EWS no Exchange](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [Operação RemoveImGroup](removeimgroup-operation.md)
    
- [SetImGroup](setimgroup.md)
    

