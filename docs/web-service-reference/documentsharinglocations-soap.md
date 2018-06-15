---
title: DocumentSharingLocations (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 394f6015-721b-4800-9286-039d430f09b3
description: O elemento DocumentSharingLocations contém uma lista de localização e informações de metadados para um local de compartilhamento de documentos.
ms.openlocfilehash: 72d1ae9f01ad45441b4e255f2fb6353be2dc8d28
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2018
ms.locfileid: "19751912"
---
# <a name="documentsharinglocations-soap"></a>DocumentSharingLocations (SOAP)

O elemento **DocumentSharingLocations** contém uma lista de localização e informações de metadados para um local de compartilhamento de documentos. 
  
```XML
<DocumentSharingLocations>
   <DocumentSharingLocation />
</DocumentSharingLocations>
```

 **DocumentSharingLocations**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DocumentSharingLocation (SOAP)](documentsharinglocation-soap.md) <br/> |Contém o local e metadados para um local de compartilhamento de documentos.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DocumentSharingLocationCollectionSetting (SOAP)](documentsharinglocationcollectionsetting-soap.md) <br/> |Representa um usuário de configuração que é uma coleção de documentação compartilhando locais e metadados.  <br/> |
   
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

