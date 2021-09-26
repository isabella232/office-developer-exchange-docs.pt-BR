---
title: DocumentSharingLocation (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 21bc388c-33be-422b-a89d-30ade0fae8f1
description: O elemento DocumentSharingLocation contém informações de localização e metadados para um local de compartilhamento de documentos.
ms.openlocfilehash: f4011dfb846d314d926ba644f4ddc2176283008a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541480"
---
# <a name="documentsharinglocation-soap"></a>DocumentSharingLocation (SOAP)

O **elemento DocumentSharingLocation** contém informações de localização e metadados para um local de compartilhamento de documentos. 
  
```XML
<DocumentSharingLocation>
   <ServiceUrl />
   <LocationUrl />
   <DisplayName />
   <SupportedFileExtensions />
   <ExternalAccessAllowed />
   <AnonymousAccessAllowed />
   <CanModifyPermissions />
   <IsDefault />
</DocumentSharingLocation>
```

 **DocumentSharingLocation**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ServiceUrl (SOAP)](serviceurl-soap.md) <br/> |Representa a URL do serviço Web de compartilhamento de documentos.  <br/> |
|[LocationUrl (SOAP)](locationurl-soap.md) <br/> |Representa a URL do local de compartilhamento de documentos.  <br/> |
|[DisplayName (SOAP)](displayname-soap.md) <br/> |Representa o nome do local de compartilhamento de documentos a ser usado na interface do usuário.  <br/> |
|[SupportedFileExtensions (SOAP)](supportedfileextensions-soap.md) <br/> |Representa as extensões de arquivo que podem ser armazenadas no local de compartilhamento de documentos.  <br/> |
|[ExternalAccessAllowed (SOAP)](externalaccessallowed-soap.md) <br/> |Indica se o local de compartilhamento de documentos está disponível para conexões externas.  <br/> |
|[AnonymousAccessAllowed (SOAP)](anonymousaccessallowed-soap.md) <br/> |Indica se o acesso ao local de compartilhamento requer um usuário autenticado.  <br/> |
|[CanModifyPermissions (SOAP)](canmodifypermissions-soap.md) <br/> |Indica se o usuário pode modificar permissões de acesso para o local de compartilhamento de documentos.  <br/> |
|[IsDefault (SOAP)](isdefault-soap.md) <br/> |Indica se o local de compartilhamento de documentos é o local de compartilhamento padrão do usuário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DocumentSharingLocations (SOAP)](documentsharinglocations-soap.md) <br/> |Contém uma lista de locais de compartilhamento de documentos e metadados.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Referência do serviço Web de Descoberta Automática para Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Elementos XML de Descoberta Automática SOAP para Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

