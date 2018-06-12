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
description: O elemento OofSettings contém as configurações de fora do escritório (OOF).
ms.openlocfilehash: d71f068ff24af22da98b6b4de090ab26d3f74f26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824649"
---
# <a name="oofsettings"></a>OofSettings

O elemento **OofSettings** contém as configurações de fora do escritório (OOF). 
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[OofState](oofstate.md) <br/> |Contém o estado de ausência temporária do usuário.  <br/> |
|[ExternalAudience](externalaudience.md) <br/> |Contém um valor que determina a quem as mensagens de ausência temporária externas são enviadas.  <br/> |
|[Duração (UserOofSettings)](duration-useroofsettings.md) <br/> |Contém a duração em que o status de ausência temporária está ativado se o elemento [OofState](oofstate.md) for definido como **agendado**. Se o elemento [OofState](oofstate.md) for definido como **habilitado** ou **desabilitado**, o valor deste elemento será ignorado.  <br/> |
|[InternalReply](internalreply.md) <br/> |Contém a resposta de ausência temporária enviada para outros usuários no domínio do usuário ou o domínio confiável.  <br/> |
|[ExternalReply](externalreply.md) <br/> |Contém a resposta de ausência temporária enviada para endereços fora do domínio ou os domínios confiáveis do destinatário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |Contém os resultados de resposta e as configurações de ausência temporária para um usuário.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/GetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação GetUserOofSettings](getuseroofsettings-operation.md)
  
[Operação SetUserOofSettings](setuseroofsettings-operation.md)

