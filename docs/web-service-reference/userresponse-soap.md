---
title: Resposta SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd
description: O elemento de resposta representa uma resposta a uma solicitação de GetUserSettings para um usuário individual.
ms.openlocfilehash: 6fcd82e06916df5acdd317cb44161c1b69e58574
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2018
ms.locfileid: "19837996"
---
# <a name="userresponse-soap"></a>Resposta SOAP)

O elemento de **resposta** representa uma resposta a uma solicitação de GetUserSettings para um usuário individual. 
  
```XML
<UserResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <RedirectTarget/>
   <UserSettingErrors/>
   <UserSettings/>
</UserResponse>
```

 **Resposta**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Representa um código de erro retornado pelo serviço de descoberta automática.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Representa uma mensagem que está associada um código de erro retornado pelo serviço de descoberta automática.  <br/> |
|[RedirectTarget (SOAP)](redirecttarget-soap.md) <br/> |Contém o destino do endereço de email ou a URL de redirecionamento.  <br/> |
|[UserSettingErrors (SOAP)](usersettingerrors-soap.md) <br/> |Representa uma coleção de informações sobre as configurações que não puderam ser retornadas.  <br/> |
|[UserSettings (SOAP)](usersettings-soap.md) <br/> |As configurações solicitadas para o usuário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ArrayOfUserResponse (SOAP)](arrayofuserresponse-soap.md) <br/> |Contém uma matriz de respostas do usuário.  <br/> |
|[UserResponses (SOAP)](userresponses-soap.md) <br/> |Contém as definições de configuração para cada usuário solicitado.  <br/> |
   
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



[Elementos de Autodiscover XML SOAP para o Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

