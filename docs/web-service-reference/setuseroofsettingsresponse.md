---
title: SetUserOofSettingsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetUserOofSettingsResponse
api_type:
- schema
ms.assetid: 8aa4025b-38df-4d63-a6a5-c3b932bec26e
description: O elemento SetUserOofSettingsResponse contém o resultado de uma tentativa de mensagem SetUserOofSettingsRequest.
ms.openlocfilehash: ab2eaaad1b7b094baad724ec56f4c26280f1f15f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825471"
---
# <a name="setuseroofsettingsresponse"></a>SetUserOofSettingsResponse

O elemento **SetUserOofSettingsResponse** contém o resultado de uma tentativa de mensagem [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) . 
  
```xml
<SetUserOofSettingsResponse>
   <ResponseMessage>...</ResponseMessage>
<SetUserOofSettingsResponse>
```

 **SetUserOofSettingsResponse**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> |Fornece informações descritivas sobre o status de resposta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
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



[Operação SetUserOofSettings](setuseroofsettings-operation.md)

