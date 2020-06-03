---
title: ResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessage
api_type:
- schema
ms.assetid: bf57265a-d354-4cd7-bbfc-d93e19cbede6
description: O elemento ResponseMessage fornece informações descritivas sobre o status de resposta para uma única entidade dentro de uma solicitação.
ms.openlocfilehash: a7f4240b1e988cb69d67118c6db58db0d7babba5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467155"
---
# <a name="responsemessage"></a>ResponseMessage

O elemento **ResponseMessage** fornece informações descritivas sobre o status de resposta para uma única entidade dentro de uma solicitação. 
  
```xml
<ResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ResponseMessage>
```

 **ResponseMessageType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**ResponseClass** <br/> | Representa o status da resposta. <br/><br/>Os seguintes valores são válidos para este atributo:  <br/><br/>-Êxito  <br/>-Aviso  <br/>-Erro  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Valores de atributo ResponseClass

|**Valor**|**Descrição**|
|:-----|:-----|
|Êxito  <br/> |Descreve uma solicitação que é atendida.  <br/> |
|Aviso  <br/> | Descreve uma solicitação que não foi processada. Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes. <br/><br/>Veja a seguir algumas possíveis causas para os avisos:  <br/><br/>– O repositório do Exchange está offline durante o lote.  <br/>– O serviço de diretório do Active Directory está offline.  <br/>-As caixas de correio são movidas.  <br/>– O banco de dados de mensagens (MDB) está offline.  <br/>-Uma senha expirou.  <br/>-Uma cota foi excedida.  <br/> |
|Erro  <br/> | Descreve uma solicitação que não pode ser atendida. <br/><br/>Veja a seguir algumas possíveis causas de erros:  <br/><br/>-Atributos ou elementos inválidos  <br/>-Atributos ou elementos fora do intervalo  <br/>– Marca desconhecida  <br/>-Atributo ou elemento não válido no contexto  <br/>– Tentativa de acesso não autorizado por qualquer cliente  <br/>-Falha do servidor em resposta a uma chamada válida do lado do cliente  <br/> <br/> As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fornece um código de erro que identifica o erro específico que a solicitação encontrou.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Não utilizado no momento e está reservado para uso futuro. Ele contém um valor de 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fornece informações adicionais de resposta de erro.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FreeBusyResponse](freebusyresponse.md) <br/> |Contém as informações de disponibilidade de um único usuário de caixa de correio. <br/> <br/> A seguir está a expressão XPath 2,0 para este elemento: <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray[i]/FreeBusyResponse` <br/> |
|[SuggestionsResponse](suggestionsresponse.md) <br/> |Contém informações de resposta e dados de sugestão para sugestões de reunião solicitadas.  <br/><br/> A seguir está a expressão XPath 2,0 para este elemento:<br/>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |Contém os resultados da resposta e as configurações de ausência temporária de um usuário.  <br/><br/> A seguir está a expressão XPath 2,0 para este elemento:  <br/><br/>  `/GetUserOofSettingsResponse` <br/> |
|[SetUserOofSettingsResponse](setuseroofsettingsresponse.md) <br/> |Contém o resultado de uma mensagem tentada [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) . <br/> <br/> A seguir está a expressão XPath 2,0 para este elemento:  <br/><br/>  `/SetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a>Comentários

O tipo **ResponseMessageType** é comum a todas as respostas de serviços Web do Exchange. O tipo **ResponseMessageType** é estendido pelos seguintes tipos complexos: 
  
- **ApplyConversationActionResponseMessageType**
    
- **AttachmentInfoResponseMessageType**
    
- **DeleteAttachmentResponseMessageType**
    
- **DeleteItemResponseMessageType**
    
- **ExpandDLResponseMessageType**
    
- **FindFolderResponseMessageType**
    
- **FindItemResponseMessageType**
    
- **FolderInfoResponseMessageType**
    
- **GetEventsResponseMessageType**
    
- **ItemInfoResponseMessageType**
    
- **ResolveNamesResponseMessageType**
    
- **SubscribeResponseMessageType**
    
- **SendNotificationResponseMessageType**
    
- **SyncFolderHierarchyResponseMessageType**
    
- **SyncFolderItemsResponseMessageType**
    
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
### <a name="version-differences"></a>Diferenças de versão

Os tipos **ApplyConversationActionResponseMessage** e **DeleteItemResponseMessageType** foram introduzidos no 15.00.0986.00 de compilação do Exchange. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserAvailability](getuseravailability-operation.md)
- [Operação SetUserOofSettings](setuseroofsettings-operation.md)
- [Operação GetUserOofSettings](getuseroofsettings-operation.md)
- [Obtendo disponibilidade do usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

