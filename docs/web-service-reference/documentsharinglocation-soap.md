---
title: DocumentSharingLocation (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 21bc388c-33be-422b-a89d-30ade0fae8f1
description: O elemento DocumentSharingLocation contém informações de metadados para um local de compartilhamento de documentos e local.
ms.openlocfilehash: d258efecb46d570138c7c2c78ed9d2fa9a275103
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751908"
---
# <a name="documentsharinglocation-soap"></a>DocumentSharingLocation (SOAP)

O elemento **DocumentSharingLocation** contém informações de metadados para um local de compartilhamento de documentos e local. 
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ServiceUrl (SOAP)](serviceurl-soap.md) <br/> |Representa a URL do documento compartilhamento de serviço web.  <br/> |
|[LocationUrl (SOAP)](locationurl-soap.md) <br/> |Representa a URL do documento local de compartilhamento.  <br/> |
|[DisplayName (SOAP)](displayname-soap.md) <br/> |Representa o nome do documento compartilhamento local a ser usado na interface de usuário.  <br/> |
|[SupportedFileExtensions (SOAP)](supportedfileextensions-soap.md) <br/> |Representa as extensões de arquivo que podem ser armazenadas no documento local de compartilhamento.  <br/> |
|[ExternalAccessAllowed (SOAP)](externalaccessallowed-soap.md) <br/> |Indica se o documento local de compartilhamento está disponível para fora de conexões.  <br/> |
|[AnonymousAccessAllowed (SOAP)](anonymousaccessallowed-soap.md) <br/> |Indica se o acesso à localização de compartilhamento requer um usuário autenticado.  <br/> |
|[CanModifyPermissions (SOAP)](canmodifypermissions-soap.md) <br/> |Indica se o usuário pode modificar permissões de acesso para o documento local de compartilhamento.  <br/> |
|[IsDefault (SOAP)](isdefault-soap.md) <br/> |Indica se o documento local de compartilhamento é o padrão do usuário local de compartilhamento.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DocumentSharingLocations (SOAP)](documentsharinglocations-soap.md) <br/> |Contém uma lista de locais e metadados de compartilhamento de documentos.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação de GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Referência de web service de descoberta automática do Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Elementos de Autodiscover XML SOAP para o Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

