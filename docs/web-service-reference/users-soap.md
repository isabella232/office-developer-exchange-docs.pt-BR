---
title: Usuários (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4e051617-4eea-47d0-871a-ea1f17a0f711
description: O elemento Users representa uma coleção de endereços de email dos usuários para os quais as configurações devem ser recuperadas.
ms.openlocfilehash: 851447a2918e365b7c5d8812a61c9d425d26ffa2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461895"
---
# <a name="users-soap"></a>Usuários (SOAP)

O elemento **Users** representa uma coleção de endereços de email dos usuários para os quais as configurações devem ser recuperadas. 
  
```XML
<Users>
   <User/>
</Users>
```

 **Usuários**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Usuário (SOAP)](user-soap.md) <br/> |Representa o endereço de email de um usuário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md) <br/> |Representa uma solicitação para recuperar as configurações especificadas de um ou mais usuários.  <br/> |
|[Solicitação (SOAP)](request-soap.md) <br/> |Contém as definições de configuração solicitadas e os usuários de destino.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)

