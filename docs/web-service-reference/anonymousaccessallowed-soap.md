---
title: AnonymousAccessAllowed (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: bf819a65-30f2-4881-a34f-cb30a9c2b6a7
description: O elemento AnonymousAccessAllowed indica se um local de compartilhamento de documentos requer um usuário autenticado.
ms.openlocfilehash: bf31b8dd4e61393539a1cba0387d1fbbc7f282d7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516122"
---
# <a name="anonymousaccessallowed-soap"></a>AnonymousAccessAllowed (SOAP)

O **elemento AnonymousAccessAllowed** indica se um local de compartilhamento de documentos requer um usuário autenticado. 
  
```XML
<AnonymousAccessAllowed /> 
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
|[DocumentSharingLocation (SOAP)](documentsharinglocation-soap.md) <br/> |Representa informações de localização e metadados para um local de compartilhamento de documentos.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor Boolean do **elemento AnonymousAccessAllowed** indica se o local de compartilhamento requer um usuário autenticado. 
  
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

