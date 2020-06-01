---
title: Operação GetSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolder
api_type:
- schema
ms.assetid: 75fee92a-a7f8-4a62-ad2b-17acbaada186
description: A operação GetSharingFolder Obtém o identificador de pasta local de uma pasta compartilhada especificada.
ms.openlocfilehash: cf66eb390b0287e89bb8402f26a2e728868a2b18
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460509"
---
# <a name="getsharingfolder-operation"></a>Operação GetSharingFolder

A operação **GetSharingFolder** Obtém o identificador de pasta local de uma pasta compartilhada especificada. 
  
## <a name="soap-headers"></a>Cabeçalhos SOAP

A operação **GetSharingFolder** pode usar os cabeçalhos SOAP listados e descritos na tabela a seguir. 
  
|**Header**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação.  <br/> |
   
## <a name="getsharingfolder-request-example"></a>Exemplo de solicitação GetSharingFolder

### <a name="getting-the-local-folder-identifier-by-specifying-the-sharedfolderid-element-of-the-folder-being-shared"></a>Obtendo o identificador de pasta local especificando o elemento SharedFolderId da pasta que está sendo compartilhada

O exemplo de código a seguir mostra como formar uma solicitação para obter o identificador da pasta local que corresponde à pasta que está sendo compartilhada. A pasta que está sendo compartilhada é identificada pelo endereço SMTP da caixa de correio que contém a pasta que está sendo compartilhada e pelo elemento [SharedFolderId](sharedfolderid.md) que representa o identificador da pasta. Neste exemplo, a pasta que está sendo compartilhada pertence a user1@contoso.com. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetSharingFolder>
      <m:SmtpAddress>user1@contoso.com</m:SmtpAddress>
      <m:SharedFolderId>AAMkA=</m:SharedFolderId>
    </m:GetSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="getting-the-local-folder-identifier-by-specifying-the-datatype-element-of-the-folder-being-shared"></a>Obtendo o identificador de pasta local especificando o elemento DataType da pasta que está sendo compartilhada

O exemplo de código a seguir mostra como formar uma solicitação para obter o identificador da pasta local que corresponde à pasta que está sendo compartilhada. A pasta que está sendo compartilhada é identificada pelo endereço SMTP da caixa de correio que contém a pasta que está sendo compartilhada e pelo elemento [DataType](datatype.md) que representa o tipo de dados nessa pasta. Neste exemplo, a pasta que está sendo compartilhada é a pasta de contatos pertencente ao user1@contoso.com. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetSharingFolder>
      <m:SmtpAddress>user1@contoso.com</m:SmtpAddress>
      <m:DataType>Contacts</m:DataType>
    </m:GetSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

Para obter informações sobre os valores possíveis do elemento **DataType** , consulte [DataType](datatype.md).
  
## <a name="successful-getsharingfolder-response"></a>Resposta GetSharingFolder bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação **GetSharingFolder** . O atributo **ID** do elemento [SharingFolderId](sharingfolderid.md) representa o identificador da pasta local na relação de compartilhamento. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Success"
                                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:SharingFolderId Id="AAMkAD=" ChangeKey="AwAAA=" />
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="getsharingfolder-error-response"></a>Resposta de erro GetSharingFolder

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro a uma solicitação **GetSharingFolder** . Neste exemplo, o erro ocorreu porque a solicitação especificou os elementos [SharingFolderId](sharingfolderid.md) e [DataType](datatype.md) . Observe que apenas um ou outro desses dois elementos pode ser especificado, mas não ambos. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Error" 
                                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:MessageText>Either DataType or SharedFolderId must be specified, but not both.</m:MessageText>
      <m:ResponseCode>ErrorInvalidGetSharingFolderRequest</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Também consulte



[GetSharingFolder](getsharingfolder.md)
  
[GetSharingFolderType](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderType.aspx)
  
[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md)
  
[GetSharingFolderResponseMessageType](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderResponseMessageType.aspx)


[Operações do EWS no Exchange](ews-operations-in-exchange.md)
  
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

