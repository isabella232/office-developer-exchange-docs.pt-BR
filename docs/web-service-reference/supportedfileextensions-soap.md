---
title: SupportedFileExtensions (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 6f73d18c-7bb1-4ab6-a23b-6d948e590b53
description: O elemento SupportedFileExtensions lista as extensões de arquivo que podem ser armazenadas em um local de compartilhamento de documentos.
ms.openlocfilehash: d783b147a25ebbe3bff59c2142012b50bd80004e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44433984"
---
# <a name="supportedfileextensions-soap"></a>SupportedFileExtensions (SOAP)

O elemento **SupportedFileExtensions** lista as extensões de arquivo que podem ser armazenadas em um local de compartilhamento de documentos. 
  
```XML
<SupportedFileExtensions /> 
```

 **ArrayOfFileExtension**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExtensãoDeArquivo (SOAP)](fileextension-soap.md) <br/> |Representa uma extensão de arquivo.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DocumentSharingLocation (SOAP)](documentsharinglocation-soap.md) <br/> |Representa informações de localização e metadados de um local de compartilhamento de documentos.  <br/> |
   
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Também consulte



[Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)


[Referência do serviço Web de descoberta automática do Exchange](autodiscover-web-service-reference-for-exchange.md)
  
[Elementos XML de descoberta automática SOAP para o Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

