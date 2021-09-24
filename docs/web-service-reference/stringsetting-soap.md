---
title: StringSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: bf7096d8-42d4-4bf5-bbdd-851af2754000
description: O elemento StringSetting representa um usuário definindo o valor do qual é da cadeia de caracteres de tipo.
ms.openlocfilehash: 16a59475c82a4088421f5916f1416ab91e7d78d6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540388"
---
# <a name="stringsetting-soap"></a>StringSetting (SOAP)

O **elemento StringSetting** representa um usuário definindo o valor do qual é da cadeia de caracteres de tipo. 
  
```XML
<StringSetting>
   <Name/>
   <Value/>
</StringSetting>
```

 **StringSetting**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Name (SOAP)](name-soap.md) <br/> |Representa um nome de configuração do usuário.  <br/> |
|[Value (SOAP)](value-soap.md) <br/> |Representa um valor de configuração do usuário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O **tipo StringSetting** estende o **tipo UserSetting.** 
  
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

