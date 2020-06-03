---
title: ExternalAccessAllowed (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 967df8c0-ee95-4202-b037-0c4b9fbbf5ee
description: O elemento ExternalAccessAllowed indica se um local de compartilhamento de documento está disponível para conexões externas.
ms.openlocfilehash: eb0ce0067a9ac9deea78b2778ce7f9e493ffb26f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457960"
---
# <a name="externalaccessallowed-soap"></a>ExternalAccessAllowed (SOAP)

O elemento **ExternalAccessAllowed** indica se um local de compartilhamento de documento está disponível para conexões externas. 
  
```XML
<ExternalAccessAllowed /> 
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DocumentSharingLocation (SOAP)](documentsharinglocation-soap.md) <br/> |Representa informações de localização e metadados de um local de compartilhamento de documentos.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor booliano do elemento **ExternalAccessAllowed** indica se o local de compartilhamento está disponível para conexões externas. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)


[Referência do serviço Web de descoberta automática do Exchange](autodiscover-web-service-reference-for-exchange.md)
  
[Elementos XML de descoberta automática SOAP para o Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

