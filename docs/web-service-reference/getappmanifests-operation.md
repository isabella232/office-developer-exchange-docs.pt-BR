---
title: Operação GetAppManifests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 21a4987c-c24d-4a6e-ace4-e81edcda6303
description: Encontre informações sobre a operação GetAppManifests EWS.
ms.openlocfilehash: 979a09d24d0c9365a92e589aa169bebf2340411b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509914"
---
# <a name="getappmanifests-operation"></a>Operação GetAppManifests

Encontre informações sobre a **operação GetAppManifests** EWS. 
  
A **operação GetAppManifests** recupera os manifestos do aplicativo. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-getappmanifests-operation"></a>Usando a operação GetAppManifests

A **operação GetAppManifests** não leva argumentos para solicitar os manifestos do aplicativo para uma caixa de correio. A resposta conterá arquivos de manifesto XML codificados com base64 para cada aplicativo instalado em uma caixa de correio. 
  
### <a name="getappmanifests-operation-soap-headers"></a>Headers SOAP da operação GetAppManifests

A **operação GetAppManifests** pode usar os headers SOAP listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Esse header é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Esse header é aplicável a uma resposta.  <br/> |
   
## <a name="getappmanifests-operation-request-example-get-the-app-manifests-for-a-mailbox"></a>Exemplo de solicitação de operação GetAppManifests: Obter os manifestos do aplicativo para uma caixa de correio

O exemplo a seguir de uma **solicitação de operação GetAppManifests** mostra como obter os manifestos do aplicativo para uma caixa de correio. O [elemento ApiVersionSupported](apiversionsupported.md) e o [elemento SchemaVersionSupported são](schemaversionsupported.md) opcionais. 
  
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
    
## <a name="successful-getappmanifests-operation-response"></a>Resposta bem-sucedida da operação GetAppManifests

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetAppManifests** para obter os manifestos do aplicativo para uma caixa de correio. 
  
> [!NOTE]
> Todos os manifestos de aplicativo base64 foram arbitrariamente truncados para preservar a capacidade de leitura. 
  
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
    
- [Aplicativos](apps.md)
    
- [Aplicativo](app.md)
    
- [Manifesto](manifest.md)
    
O corpo SOAP de resposta também pode conter o seguinte elemento:
  
- [Manifestos](manifests.md)
    
## <a name="getappmanifests-operation-error-response"></a>Resposta de erro da operação GetAppManifests

Os erros retornados para essa operação estão relacionados a um formato inválido dos parâmetros de entrada ou são erros genéricos do EWS. Para códigos de erro genéricos para EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).
  
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

## <a name="see-also"></a>Confira também

- [Operações EWS em Exchange](ews-operations-in-exchange.md)
    
- [Operação DisableApp](disableapp-operation.md)
    
- [Operação InstallApp](installapp-operation.md)
    
- [Operação UninstallApp](uninstallapp-operation.md)
    
- [Operação GetAppMarketplaceUrl](getappmarketplaceurl-operation.md)
    

