---
title: Operação InstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 596eae95-3e78-489a-8bb2-d2dd4a026405
description: Encontre informações sobre a operação InstallApp EWS.
ms.openlocfilehash: 87e6f1caddd6949d5dc98edc074acd365de818d9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515576"
---
# <a name="installapp-operation"></a>Operação InstallApp

Encontre informações sobre a **operação InstallApp** EWS. 
  
A **operação InstallApp** instala um aplicativo de email para Outlook em uma caixa de correio. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-installapp-operation"></a>Usando a operação InstallApp

A **operação InstallApp** tem um único argumento que identifica um aplicativo de email a ser instalado. O argumento contém o manifesto codificado com base64 para um aplicativo de email. 
  
### <a name="installapp-operation-soap-headers"></a>Headers SOAP da operação InstallApp

A **operação InstallApp** pode usar os headers SOAP listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Esse header é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Esse header é aplicável a uma resposta.  <br/> |
   
## <a name="installapp-operation-request-example-install-a-mail-app-in-a-mailbox"></a>Exemplo de solicitação de operação installApp: Instalar um aplicativo de email em uma caixa de correio

O exemplo a seguir de uma **solicitação de** operação installApp mostra como instalar um aplicativo de email para Outlook. O manifesto do aplicativo pode ser encontrado usando a [operação GetAppManifests.](getappmanifests-operation.md)
  
> [!NOTE]
> O manifesto do aplicativo codificado com base64 foi arbitrariamente truncado para preservar a capacidade de leitura e não representa um manifesto válido. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

O corpo SOAP de solicitação contém os seguintes elementos:
  
- [InstallApp](installapp.md)
    
- [Manifesto](manifest.md)
    
## <a name="successful-installapp-operation-response"></a>Resposta bem-sucedida da operação InstallApp

O exemplo a seguir mostra uma resposta bem-sucedida a uma **solicitação de** operação installApp para instalar um aplicativo de email. 
  
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
      <InstallAppResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>
```

O corpo SOAP de resposta contém os seguintes elementos:
  
- [InstallAppResponse](installappresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="installapp-operation-error-response"></a>Resposta de erro da operação InstallApp

O exemplo a seguir mostra uma resposta de erro a uma **solicitação de operação InstallApp.** Esta é uma resposta a uma solicitação que contém um manifesto inválido. 
  
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
      <InstallAppResponse ResponseClass="Error" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>This app can't be installed. Missing OfficeApp element.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>

```

O corpo SOAP da resposta de erro contém os seguintes elementos:
  
- [InstallAppResponse](installappresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Confira também

- [Operações EWS em Exchange](ews-operations-in-exchange.md)
    
- [Operação DisableApp](disableapp-operation.md)
    
- [Operação UninstallApp](uninstallapp-operation.md)
    
- [GetAppManifests](getappmanifests.md)
    
- [Operação GetAppMarketplaceUrl](getappmarketplaceurl-operation.md)
    

