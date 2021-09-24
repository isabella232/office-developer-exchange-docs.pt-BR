---
title: GetUserOofSettingsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetUserOofSettingsResponse
api_type:
- schema
ms.assetid: 011cb38b-da3c-4b1b-8836-a6b212b511f6
description: O elemento GetUserOofSettingsResponse contém a mensagem de resposta e as configurações Fora de Office (OOF) para um usuário.
ms.openlocfilehash: 57e24dd4aa8ea10955cb309cad76f35cbb9395d4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526124"
---
# <a name="getuseroofsettingsresponse"></a>GetUserOofSettingsResponse

O **elemento GetUserOofSettingsResponse** contém a mensagem de resposta e as configurações Fora de Office (OOF) para um usuário. 
  
```xml
<GetUserOofSettingsResponse>
   <ResponseMessage>...</ResponseMessage>
   <OofSettings>...</OofSettings>
   <AllowExternalOof>...</AllowExternalOof>
</GetUserOofSettingsResponse>
```

 **GetUserOofSettingsResponse**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> |Fornece informações descritivas sobre o status da resposta.  <br/> |
|[OofSettings](oofsettings.md) <br/> |Contém as configurações OOF.  <br/> |
|[AllowExternalOof](allowexternaloof.md) <br/> |Contém um valor que identifica a quem as mensagens OOF externas são enviadas.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
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

