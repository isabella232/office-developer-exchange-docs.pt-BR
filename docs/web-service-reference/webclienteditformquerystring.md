---
title: WebClientEditFormQueryString
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- WebClientEditFormQueryString
api_type:
- schema
ms.assetid: 9e571021-d58f-424b-8db2-48cf683533dc
description: O elemento WebClientEditFormQueryString representa uma URL para concatenar ao ponto de extremidade Outlook Web App para editar um item no Outlook Web App.
ms.openlocfilehash: d6e67d34de5b58624060beaadb4db1c322230bc0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537291"
---
# <a name="webclienteditformquerystring"></a>WebClientEditFormQueryString

O **elemento WebClientEditFormQueryString** representa uma URL para concatenar ao ponto de extremidade Outlook Web App para editar um item no Outlook Web App. 
  
```XML
<WebClientEditFormQueryString/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Representa um Exchange de calendário.  <br/> |
|[Contato](contact.md) <br/> |Representa um Exchange de contato.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[Item](item.md) <br/> |Representa um item no Exchange store.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no Exchange store.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no Exchange store.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no Exchange store.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no Exchange store.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma Exchange de email.  <br/> |
|[Item de postagem](postitem.md) <br/> |Representa um item post no Exchange store.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no Exchange store.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa uma cadeia de caracteres será necessário se esse elemento for usado.
  
## <a name="remarks"></a>Comentários

Para versões do Exchange a partir do Exchange Server 2013, incluindo Exchange Online, use as informações do [elemento WebClientReadFormQueryString](webclientreadformquerystring.md) para abrir um item de rascunho no Outlook Web App e, em seguida, usar a interface do usuário para editar o item de rascunho. O **elemento WebClientEditFormQueryString** não é aplicável às versões do Exchange a partir do Exchange Server 2013, incluindo Exchange Online. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

