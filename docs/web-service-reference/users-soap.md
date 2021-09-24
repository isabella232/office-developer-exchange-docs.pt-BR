---
title: Users (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 4e051617-4eea-47d0-871a-ea1f17a0f711
description: O elemento Users representa uma coleção de endereços de email dos usuários para os quais as configurações devem ser recuperadas.
ms.openlocfilehash: eabf0d2cd38396e907ca467596c2e55d1eb78e02
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538517"
---
# <a name="users-soap"></a>Users (SOAP)

O **elemento Users** representa uma coleção de endereços de email dos usuários para os quais as configurações devem ser recuperadas. 
  
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
|[User (SOAP)](user-soap.md) <br/> |Representa o endereço de email de um usuário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md) <br/> |Representa uma solicitação para recuperar as configurações especificadas para um ou mais usuários.  <br/> |
|[Request (SOAP)](request-soap.md) <br/> |Contém as configurações solicitadas e os usuários de destino.  <br/> |
   
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



[Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)

