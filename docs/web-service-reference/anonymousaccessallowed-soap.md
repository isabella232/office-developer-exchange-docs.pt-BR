---
title: AnonymousAccessAllowed (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: bf819a65-30f2-4881-a34f-cb30a9c2b6a7
description: O elemento AnonymousAccessAllowed indica se um local de compartilhamento de documento requer que um usuário autenticado.
ms.openlocfilehash: 7ca208aa0d75b254463400a5e207079d722fc0a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751096"
---
# <a name="anonymousaccessallowed-soap"></a>AnonymousAccessAllowed (SOAP)

O elemento **AnonymousAccessAllowed** indica se um local de compartilhamento de documento requer que um usuário autenticado. 
  
```XML
<AnonymousAccessAllowed /> 
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DocumentSharingLocation (SOAP)](documentsharinglocation-soap.md) <br/> |Representa informações de local e metadados para um local de compartilhamento de documentos.  <br/> |
   
## <a name="text-value"></a>Text value

O valor booliano do elemento **AnonymousAccessAllowed** indica se o local de compartilhamento requer um usuário autenticado. 
  
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

