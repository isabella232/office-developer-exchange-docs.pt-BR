---
title: Solicitação (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75696436-997e-49f1-a31b-eb9a8c3526f3
description: O elemento de solicitação contém as definições de configuração solicitado e os usuários de destino.
ms.openlocfilehash: dfea33786066dd7803d0fd061cbb87bb06d11531
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825125"
---
# <a name="request-soap"></a>Solicitação (SOAP)

O elemento de **solicitação** contém as definições de configuração solicitado e os usuários de destino. 
  
```XML
<Request>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</Request>
```

 **GetUserSettingsRequest**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Usuários (SOAP)](users-soap.md) <br/> |Representa uma coleção de endereços de email dos usuários cujas configurações devem ser recuperadas.  <br/> |
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Contém os nomes das definições de configuração solicitada.  <br/> |
|[RequestedVersion (SOAP)](requestedversion-soap.md) <br/> |Especifica a versão de servidor específico que o provedor gostaria de usar.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetUserSettingsRequestMessage (SOAP)](getusersettingsrequestmessage-soap.md) <br/> |Representa uma solicitação de [operação GetUserSettings (SOAP)](getusersettings-operation-soap.md) .  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação de GetUserSettings (SOAP)](getusersettings-operation-soap.md)

