---
title: Userresponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd
description: O elemento userresponse representa uma resposta a uma solicitação GetUserSettings para um usuário individual.
ms.openlocfilehash: 73848cb19d9c859e07216f354965ac4051d0d20c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468898"
---
# <a name="userresponse-soap"></a>Userresponse (SOAP)

O elemento **userresponse** representa uma resposta a uma solicitação GetUserSettings para um usuário individual. 
  
```XML
<UserResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <RedirectTarget/>
   <UserSettingErrors/>
   <UserSettings/>
</UserResponse>
```

 **Userresponse**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Representa um código de erro retornado pelo serviço de descoberta automática.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Representa uma mensagem que é associada a um código de erro retornado pelo serviço de descoberta automática.  <br/> |
|[RedirectTarget (SOAP)](redirecttarget-soap.md) <br/> |Contém o destino da URL de redirecionamento ou endereço de email.  <br/> |
|[UserSettingErrors (SOAP)](usersettingerrors-soap.md) <br/> |Representa uma coleção de informações sobre as configurações que não puderam ser retornadas.  <br/> |
|[UserSettings (SOAP)](usersettings-soap.md) <br/> |As configurações solicitadas para o usuário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ArrayOfUserResponse (SOAP)](arrayofuserresponse-soap.md) <br/> |Contém uma matriz de respostas do usuário.  <br/> |
|[Userresponses (SOAP)](userresponses-soap.md) <br/> |Contém as definições de configuração para cada usuário solicitado.  <br/> |
   
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Elementos XML de descoberta automática SOAP para o Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

