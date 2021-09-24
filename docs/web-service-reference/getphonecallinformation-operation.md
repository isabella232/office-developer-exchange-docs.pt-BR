---
title: Operação GetPhoneCallInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetPhoneCallInformation
api_type:
- schema
ms.assetid: 418bd6ca-39d9-49a9-841e-7a71ede1fa51
description: A operação GetPhoneCallInformation retorna informações sobre a chamada telefônica especificada.
ms.openlocfilehash: 7cb9ecbb30e6cdd4d85b60215f40e0be5f4aaa84
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539954"
---
# <a name="getphonecallinformation-operation"></a>Operação GetPhoneCallInformation

A **operação GetPhoneCallInformation** retorna informações sobre a chamada telefônica especificada. 
  
## <a name="getphonecallinformation-request-example"></a>Exemplo de solicitação GetPhoneCallInformation

### <a name="description"></a>Descrição

O exemplo a seguir de uma **solicitação GetPhoneCallInformation** mostra como formar uma solicitação para obter informações sobre uma chamada telefônica específica. 
  
### <a name="code"></a>Código

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetPhoneCallInformation>
      <m:PhoneCallId Id="NDDY5uY29y9t"/>
    </m:GetPhoneCallInformation>
  </soap:Body>
</soap:Envelope>
```

## <a name="getphonecallinformation-response-example"></a>Exemplo de resposta GetPhoneCallInformation

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida à **solicitação GetPhoneCallInformation.** A resposta representa uma chamada telefônica que está conectada no momento. 
  
### <a name="code"></a>Código

```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetPhoneCallInformationResponse ResponseClass="Success" 
                                     xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <m:PhoneCallInformation xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
        <t:PhoneCallState xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">Connected</t:PhoneCallState>
        <t:ConnectionFailureCause xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">None</t:ConnectionFailureCause>
      </m:PhoneCallInformation>
    </GetPhoneCallInformationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>Confira também

- [Operações EWS em Exchange](ews-operations-in-exchange.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

