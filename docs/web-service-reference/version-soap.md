---
title: Version (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 47c9216e-6bfe-48c8-a27a-26f70db8e8d5
description: O elemento Version representa uma descrição da versão do produto do servidor.
ms.openlocfilehash: 67935bb97ce5a6faab3ae26ec03a842794d539e0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541627"
---
# <a name="version-soap"></a>Version (SOAP)

O **elemento Version** representa uma descrição da versão do produto do servidor. 
  
```XML
<Version/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ServerVersionInfo (SOAP)](serverversioninfo-soap.md) <br/> |Contém a versão do servidor que processou a solicitação.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor do elemento **Version** é uma descrição da versão do produto do servidor. 
  
## <a name="remarks"></a>Comentários

O **elemento Version** está contido no header SOAP de uma resposta. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
  
[Operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

