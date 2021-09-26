---
title: UserSettingErrors (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: a9b94bae-cab9-412d-a811-801e849ed6c5
description: O elemento UserSettingErrors representa uma coleção de informações sobre configurações que não puderam ser retornadas.
ms.openlocfilehash: dfcd2a0475857d95d1a7dadb3cb65b544e0f2c5d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541683"
---
# <a name="usersettingerrors-soap"></a>UserSettingErrors (SOAP)

O **elemento UserSettingErrors** representa uma coleção de informações sobre configurações que não puderam ser retornadas. 
  
```XML
<UserSettingErrors>
    <UserSettingError/>
</UserSettingErrors>
```

 **UserSettingErrors**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UserSettingError (SOAP)](usersettingerror-soap.md) <br/> |Representa um erro retornado durante a recuperação de uma configuração do usuário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UserResponse (SOAP)](userresponse-soap.md) <br/> |Representa uma resposta a uma solicitação GetUserSettings para um usuário individual.  <br/> |
   
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



[Elementos XML de Descoberta Automática SOAP para Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

