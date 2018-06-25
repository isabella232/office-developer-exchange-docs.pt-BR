---
title: Operação CreateUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateUserConfiguration
api_type:
- schema
ms.assetid: eb5b8ab6-9743-481c-aac9-f9aa889bd353
description: A operação CreateUserConfiguration cria um objeto de configuração do usuário em uma pasta.
ms.openlocfilehash: 5f0eb7d18736008af39199cbc52cc3a6e6abda09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751623"
---
# <a name="createuserconfiguration-operation"></a>Operação CreateUserConfiguration

A operação **CreateUserConfiguration** cria um objeto de configuração do usuário em uma pasta. 
  
## <a name="createuserconfiguration-request-example"></a>Exemplo de solicitação de CreateUserConfiguration

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de **CreateUserConfiguration** mostra como formar uma solicitação para criar um objeto de configuração do usuário na pasta Rascunhos. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xs="http://www.w3.org/2001/XMLSchema">
  
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:CreateUserConfiguration>
      <m:UserConfiguration>
        <t:UserConfigurationName Name="TestConfig">
          <t:DistinguishedFolderId Id="drafts">
          </t:DistinguishedFolderId>
        </t:UserConfigurationName>
        <t:Dictionary>
          <t:DictionaryEntry>
            <t:DictionaryKey>
              <t:Type>String</t:Type>
              <t:Value>PhoneNumber</t:Value>
            </t:DictionaryKey>
            <t:DictionaryValue>
              <t:Type>String</t:Type>
              <t:Value>555-555-1111</t:Value>
            </t:DictionaryValue>
          </t:DictionaryEntry>
        </t:Dictionary>
      </m:UserConfiguration>  
    </m:CreateUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

## <a name="createuserconfiguration-response-example"></a>Exemplo de resposta CreateUserConfiguration

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida à solicitação **CreateUserConfiguration** . 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateUserConfigurationResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateUserConfigurationResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:CreateUserConfigurationResponseMessage>
      </m:ResponseMessages>
    </m:CreateUserConfigurationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>Confira também



[Operações do EWS no Exchange](ews-operations-in-exchange.md)
  
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

