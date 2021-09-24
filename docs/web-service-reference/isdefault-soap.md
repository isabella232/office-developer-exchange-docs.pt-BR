---
title: IsDefault (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 7358bb88-c441-4f2c-9647-c030e7303e8a
description: O elemento IsDefault indica se um local de compartilhamento de documentos é o local de compartilhamento padrão do usuário.
ms.openlocfilehash: cf8547dc017a1470406f312214fa8e532083ef9e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539497"
---
# <a name="isdefault-soap"></a>IsDefault (SOAP)

O **elemento IsDefault** indica se um local de compartilhamento de documentos é o local de compartilhamento padrão do usuário. 
  
```XML
<IsDefault /> 
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

O valor Boolean do **elemento IsDefault** indica se o local de compartilhamento é o local de compartilhamento padrão do usuário. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)


[Referência do serviço Web de Descoberta Automática para Exchange](autodiscover-web-service-reference-for-exchange.md)
  
[Elementos XML de Descoberta Automática SOAP para Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

