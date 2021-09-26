---
title: GetUserSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 832a9211-d2d5-4a49-bcb3-1dc6dc3904ed
description: O elemento GetUserSettingsRequest representa uma solicitação para recuperar as configurações especificadas para um ou mais usuários.
ms.openlocfilehash: ccbcd67d4fdcb98be08acfecbf2ae066a91d65d2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547390"
---
# <a name="getusersettingsrequest-soap"></a>GetUserSettingsRequest (SOAP)

O **elemento GetUserSettingsRequest** representa uma solicitação para recuperar as configurações especificadas para um ou mais usuários. 
  
```XML
<GetUserSettingsRequest>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetUserSettingsRequest>
```

 **GetUserSettingsRequest**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Users (SOAP)](users-soap.md) <br/> |Representa uma coleção de endereços de email dos usuários para os quais as configurações devem ser recuperadas.  <br/> |
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Contém os nomes das configurações solicitadas.  <br/> |
|[RequestedVersion (SOAP)](requestedversion-soap.md) <br/> |Especifica a versão específica do servidor que o provedor gostaria de usar.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
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

