---
title: UserSettingError (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: abb175c5-4f38-4dcc-81e3-b511686862eb
description: O elemento UserSettingError representa um erro retornado como resultado de uma tentativa de obter uma configuração de usuário.
ms.openlocfilehash: 61603038ce93780f690d72226b1356b239d2002d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468604"
---
# <a name="usersettingerror-soap"></a>UserSettingError (SOAP)

O elemento **UserSettingError** representa um erro retornado como resultado de uma tentativa de obter uma configuração de usuário. 
  
```XML
<UserSettingError>
    <ErrorCode/>
    <ErrorMessage/>
    <SettingName/>
</UserSettingError>
```

 **UserSettingError**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Representa um código de erro retornado pelo serviço de descoberta automática.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Pasta uma mensagem associada a um código de erro retornado pelo serviço de descoberta automática.  <br/> |
|[SettingName (SOAP)](settingname-soap.md) <br/> |Representa o nome de uma configuração do usuário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UserSettingErrors (SOAP)](usersettingerrors-soap.md) <br/> |Representa uma coleção de informações sobre as configurações que não puderam ser retornadas.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Também consulte



[Elementos XML de descoberta automática SOAP para o Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

