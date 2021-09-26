---
title: OofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- OofSettings
api_type:
- schema
ms.assetid: 8f37d174-db11-427c-bbed-fdde754a60c7
description: O elemento OofSettings contém as configurações Out of Office (OOF).
ms.openlocfilehash: 0a612cacb69464dfda3c1f235c32f569d3e45775
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543167"
---
# <a name="oofsettings"></a>OofSettings

O **elemento OofSettings** contém as configurações Out of Office (OOF). 
  
[GetUserOofSettingsResponse](getuseroofsettingsresponse.md)
  
[OofSettings](oofsettings.md)
  
```xml
<OofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</OofSettings>
```

 **UserOofSettings**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[OofState](oofstate.md) <br/> |Contém o estado OOF do usuário.  <br/> |
|[ExternalAudience](externalaudience.md) <br/> |Contém um valor que determina para quem as mensagens OOF externas são enviadas.  <br/> |
|[Duration (UserOofSettings)](duration-useroofsettings.md) <br/> |Contém a duração para a qual o status OOF está habilitado se [o elemento OofState](oofstate.md) estiver definido como **Scheduled**. Se o [elemento OofState](oofstate.md) estiver definido como **Habilitado** ou **Desabilitado,** o valor desse elemento será ignorado.  <br/> |
|[InternalReply](internalreply.md) <br/> |Contém a resposta OOF enviada a outros usuários no domínio ou domínio confiável do usuário.  <br/> |
|[ExternalReply](externalreply.md) <br/> |Contém a resposta OOF enviada a endereços fora do domínio do destinatário ou domínios confiáveis.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |Contém os resultados da resposta e as configurações OOF para um usuário.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/GetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserOofSettings](getuseroofsettings-operation.md)
  
[Operação SetUserOofSettings](setuseroofsettings-operation.md)

