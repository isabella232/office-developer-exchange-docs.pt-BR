---
title: Operação GetAppManifests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 21a4987c-c24d-4a6e-ace4-e81edcda6303
description: Encontre informações sobre a operação do EWS do GetAppManifests.
ms.openlocfilehash: 4d4c1d32f14cf144335ddfdf8c9cd4c88a4421d0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463003"
---
# <a name="getappmanifests-operation"></a>Operação GetAppManifests

Encontre informações sobre a operação do EWS do **GetAppManifests** . 
  
A operação **GetAppManifests** recupera manifestos de aplicativos. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-getappmanifests-operation"></a>Usando a operação GetAppManifests

A operação **GetAppManifests** não usa argumentos para solicitar os manifestos de aplicativo para uma caixa de correio. A resposta conterá arquivos de manifesto XML codificados em base64 para cada aplicativo instalado em uma caixa de correio. 
  
### <a name="getappmanifests-operation-soap-headers"></a>Cabeçalhos SOAP de operação GetAppManifests

A operação **GetAppManifests** pode usar os cabeçalhos SOAP listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Este cabeçalho é aplicável a uma resposta.  <br/> |
   
## <a name="getappmanifests-operation-request-example-get-the-app-manifests-for-a-mailbox"></a>Exemplo de solicitação de operação GetAppManifests: obter os manifestos de aplicativo para uma caixa de correio

O exemplo a seguir de uma solicitação de operação **GetAppManifests** mostra como obter os manifestos de aplicativo para uma caixa de correio. O elemento [ApiVersionSupported](apiversionsupported.md) e o elemento [SchemaVersionSupported](schemaversionsupported.md) são opcionais. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013_SP1" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:GetAppManifests>
        <m:ApiVersionSupported>1.1</m:ApiVersionSupported>
        <m:SchemaVersionSupported>1.1</m:SchemaVersionSupported>
      </m:GetAppManifests>
   </soap:Body>
</soap:Envelope>

```

O corpo SOAP de solicitação contém o seguinte elemento:
  
- [GetAppManifests](getappmanifests.md)
    
- [ApiVersionSupported](apiversionsupported.md)
    
- [SchemaVersionSupported](schemaversionsupported.md)
    
## <a name="successful-getappmanifests-operation-response"></a>Resposta de operação GetAppManifests bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetAppManifests** para obter os manifestos de aplicativo para uma caixa de correio. 
  
> [!NOTE]
> Todos os manifestos de aplicativos Base64 foram truncados arbitrariamente para preservar a legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="07" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppManifestsResponse ResponseClass="Success" 
                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <m:Apps xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
          <t:App xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
            <t:Manifest>WNlQXBwPg==</t:Manifest>
          </t:App>
         </m:Apps>
      </GetAppManifestsResponse>
   </s:Body>
</s:Envelope>
```

O corpo SOAP de resposta contém os seguintes elementos:
  
- [GetAppManifestsResponse](getappmanifestsresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [Apps](apps.md)
    
- [App](app.md)
    
- [Manifesto](manifest.md)
    
O corpo SOAP de resposta também pode conter o seguinte elemento:
  
- [Manifestos](manifests.md)
    
## <a name="getappmanifests-operation-error-response"></a>Resposta de erro de operação GetAppManifests

Os erros retornados para esta operação estão relacionados a um formato inválido dos parâmetros de entrada ou são erros genéricos do EWS. Para códigos de erro genéricos para EWS e específicos para esta operação, consulte [ResponseCode](responsecode.md).
  
```
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="07"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetAppManifestsResponse ResponseClass="Error"
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>The apiVersionSupported parameter is invalid. 
                   It should be in the form of major version, minor 
                   version, separated by '.', for example '2.34'.</MessageText>
      <ResponseCode>ErrorInvalidRequest</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetAppManifestsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a>Também consulte

- [Operações do EWS no Exchange](ews-operations-in-exchange.md)
    
- [Operação DisableApp](disableapp-operation.md)
    
- [Operação InstallApp](installapp-operation.md)
    
- [Operação UninstallApp](uninstallapp-operation.md)
    
- [Operação GetAppMarketplaceUrl](getappmarketplaceurl-operation.md)
    

