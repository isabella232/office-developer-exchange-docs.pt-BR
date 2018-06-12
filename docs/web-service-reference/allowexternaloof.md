---
title: AllowExternalOof
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllowExternalOof
api_type:
- schema
ms.assetid: e5387172-5b92-4bb1-8394-180e9c7ff771
description: O elemento AllowExternalOof contém um valor que identifica a quem as mensagens de ausência temporária externas são enviadas.
ms.openlocfilehash: 1c87a51676bf6e44b2e650a4e973d0ab89a52e31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751084"
---
# <a name="allowexternaloof"></a>AllowExternalOof

O elemento **AllowExternalOof** contém um valor que identifica a quem as mensagens de ausência temporária externas são enviadas. 
  
- [GetUserOofSettingsResponse](getuseroofsettingsresponse.md)
  
- [AllowExternalOof](allowexternaloof.md)
  
```xml
<AllowExternalOof>None or Known or All</AllowExternalOof>
```

 **ExternalAudience**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |Contém os resultados de resposta e as configurações de ausência temporária para um usuário.  <br/> |
   
## <a name="text-value"></a>Text value

Um valor de texto é necessário para esse elemento. A tabela a seguir lista os valores possíveis para esse elemento.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|**None** <br/> |Remetentes de email fora da organização do usuário da caixa de correio que enviar mensagens para o usuário não receberá uma resposta de mensagem de ausência temporária externa.  <br/> |
|**Conhecidos** <br/> |Remetentes de email fora da organização do usuário da caixa de correio que enviar mensagens para o usuário receberá uma resposta de mensagem de ausência temporária externa apenas se o remetente está no Exchange do usuário armazenam a lista de contatos.  <br/> |
|**All** <br/> |Remetentes de email fora da organização do usuário da caixa de correio que enviar mensagens para o usuário receberá uma resposta de mensagem de ausência temporária externa.  <br/> |
   
## <a name="remarks"></a>Coment�rios

Esse elemento compartilha o mesmo tipo de elemento [ExternalAudience](externalaudience.md) . 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação GetUserOofSettings](getuseroofsettings-operation.md) 
- [Operação SetUserOofSettings](setuseroofsettings-operation.md)

