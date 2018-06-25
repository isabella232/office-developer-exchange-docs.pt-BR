---
title: Operação InstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 596eae95-3e78-489a-8bb2-d2dd4a026405
description: Encontre informações sobre o EWS InstallApp operação.
ms.openlocfilehash: ccc5d2dde949070bae905ff1ebb182c892f07fcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823951"
---
# <a name="installapp-operation"></a>Operação InstallApp

Encontre informações sobre a operação de EWS **InstallApp** . 
  
A operação **InstallApp** instala um aplicativo de email para o Outlook em uma caixa de correio. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-installapp-operation"></a>Usando a operação InstallApp

A operação **InstallApp** aceita um argumento único que identifica um aplicativo de email para instalar. O argumento contém o manifesto codificado na base64 para um aplicativo de email. 
  
### <a name="installapp-operation-soap-headers"></a>Cabeçalhos SOAP InstallApp operação

A operação **InstallApp** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Este cabeçalho é aplicável a uma resposta.  <br/> |
   
## <a name="installapp-operation-request-example-install-a-mail-app-in-a-mailbox"></a>Exemplo de solicitação de operação InstallApp: instalar um aplicativo de email em uma caixa de correio

O exemplo a seguir de uma solicitação de operação **InstallApp** mostra como instalar um aplicativo de email para Outlook. O manifesto do aplicativo pode ser encontrado usando a [operação GetAppManifests](getappmanifests-operation.md).
  
> [!NOTE]
> O manifesto do aplicativo codificado na base64 foi truncado arbitrariamente para preservar a legibilidade e não representam um manifesto válido. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:InstallApp>
         <m:Manifest>TUwiIC8+CiAgPC9SdWxlPgo8L09mZmljZUFwcD4=</m:Manifest>
      </m:InstallApp>
   </soap:Body>
</soap:Envelope>

```

A solicitação de corpo SOAP contém os seguintes elementos:
  
- [InstallApp](installapp.md)
    
- [Manifesto](manifest.md)
    
## <a name="successful-installapp-operation-response"></a>Resposta de operação InstallApp bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **InstallApp** para instalar um aplicativo de email. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <InstallAppResponse ResponseClass="Success" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>
```

A resposta SOAP body contém os seguintes elementos:
  
- [InstallAppResponse](installappresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="installapp-operation-error-response"></a>Resposta de erro de operação InstallApp

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **InstallApp** . Esta é uma resposta a uma solicitação que contém um manifesto inválido. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <InstallAppResponse ResponseClass="Error" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>This app can't be installed. Missing OfficeApp element.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>

```

A resposta de erro corpo SOAP contém os seguintes elementos:
  
- [InstallAppResponse](installappresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Confira também

- [Operações do EWS no Exchange](ews-operations-in-exchange.md)
    
- [Operação DisableApp](disableapp-operation.md)
    
- [Operação UninstallApp](uninstallapp-operation.md)
    
- [GetAppManifests](getappmanifests.md)
    
- [Operação GetAppMarketplaceUrl](getappmarketplaceurl-operation.md)
    

