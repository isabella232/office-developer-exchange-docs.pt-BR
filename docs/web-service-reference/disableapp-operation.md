---
title: Operação DisableApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 211731a3-2470-49af-bda3-1ddfc15a8e46
description: Encontre informações sobre a operação do EWS do DisableApp.
ms.openlocfilehash: 8e1f3a257a70c042a01ed70da97cfa0573a2d454
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462063"
---
# <a name="disableapp-operation"></a>Operação DisableApp

Encontre informações sobre a operação do EWS do **DisableApp** . 
  
A operação **DisableApp** desabilita um aplicativo de email para o Outlook. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-disableapp-operation"></a>Usando a operação DisableApp

A operação **DisableApp** leva dois argumentos na solicitação que identificam o aplicativo de email a ser desabilitado e o motivo pelo qual ele foi desabilitado. 
  
### <a name="disableapp-operation-soap-headers"></a>Cabeçalhos SOAP de operação DisableApp

A operação **DisableApp** pode usar os cabeçalhos SOAP listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Este cabeçalho é aplicável a uma resposta.  <br/> |
   
## <a name="disableapp-operation-request-example-disable-a-mail-app-installed-in-a-mailbox"></a>Exemplo de solicitação de operação DisableApp: desabilitar um aplicativo de email instalado em uma caixa de correio

O exemplo a seguir de uma solicitação de operação **DisableApp** mostra como um aplicativo de email desabilitado. O identificador do aplicativo pode ser encontrado no manifesto do aplicativo que é retornado em uma resposta de [operação GetAppManifests](getappmanifests-operation.md) . 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:DisableApp>
         <m:ID>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</m:ID>
         <m:DisableReason>NoReason</m:DisableReason>
      </m:DisableApp>
   </soap:Body>
</soap:Envelope>
```

O corpo SOAP de solicitação contém os seguintes elementos:
  
- [DisableApp](disableapp.md)
    
- [ID (cadeia de caracteres)](id-string.md)
    
- [DisableReason](disablereason.md)
    
## <a name="successful-disableapp-operation-response"></a>Resposta de operação DisableApp bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **DisableApp** para desabilitar um aplicativo de email. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <DisableAppResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </DisableAppResponse>
   </s:Body>
</s:Envelope>
```

O corpo SOAP de resposta contém os seguintes elementos:
  
- [DisableAppResponse](disableappresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="disableapp-operation-error-response"></a>Resposta de erro de operação DisableApp

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **DisableApp** . Esta é uma resposta a uma solicitação para desabilitar um aplicativo de email que não está instalado em uma caixa de correio. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="556" MinorBuildNumber="14" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <DisableAppResponse ResponseClass="Error" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Extension ID 1C50226D-04B5-4AB2-9FCD-42E236B59E4A can't be found.</MessageText>
         <ResponseCode>ErrorExtensionNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </DisableAppResponse>
   </s:Body>
</s:Envelope>
```

O corpo SOAP de resposta de erro contém os seguintes elementos:
  
- [DisableAppResponse](disableappresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Para obter códigos de erro adicionais genéricos para o EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Confira também

- [Operações do EWS no Exchange](ews-operations-in-exchange.md)   
- [Operação InstallApp](installapp-operation.md)   
- [Operação UninstallApp](uninstallapp-operation.md)   
- [GetAppManifests](getappmanifests.md)   
- [Operação GetAppMarketplaceUrl](getappmarketplaceurl-operation.md)   
- [Suplementos do Outlook](https://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    

