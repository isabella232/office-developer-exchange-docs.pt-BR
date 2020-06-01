---
title: OofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OofSettings
api_type:
- schema
ms.assetid: 8f37d174-db11-427c-bbed-fdde754a60c7
description: O elemento OofSettings contém as configurações de ausência temporária (OOF).
ms.openlocfilehash: c1b214fd8bfab5b7a82d41a5187cf6e0fc4ba79c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467190"
---
# <a name="oofsettings"></a>OofSettings

O elemento **OofSettings** contém as configurações de ausência temporária (OOF). 
  
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
|[OofState](oofstate.md) <br/> |Contém o estado de ausência temporária do usuário.  <br/> |
|[ExternalAudience](externalaudience.md) <br/> |Contém um valor que determina a quem mensagens externas OOF são enviadas.  <br/> |
|[Duração (UserOofSettings)](duration-useroofsettings.md) <br/> |Contém a duração para a qual o status de ausência temporária é habilitado se o elemento [OofState](oofstate.md) estiver definido como **agendado**. Se o elemento [OofState](oofstate.md) estiver definido como **Enabled** ou **Disabled**, o valor desse elemento será ignorado.  <br/> |
|[InternalReply](internalreply.md) <br/> |Contém a resposta de ausência temporária enviada a outros usuários no domínio do usuário ou domínio confiável.  <br/> |
|[ExternalReply](externalreply.md) <br/> |Contém a resposta de ausência temporária enviada para endereços fora do domínio do destinatário ou domínios confiáveis.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |Contém os resultados da resposta e as configurações de ausência temporária de um usuário.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/GetUserOofSettingsResponse` <br/> |
   
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

