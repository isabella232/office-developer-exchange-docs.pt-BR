---
title: WebClientReadFormQueryString
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- WebClientReadFormQueryString
api_type:
- schema
ms.assetid: 13e8871a-32a6-4bb9-9493-864c4c07efff
description: O elemento WebClientReadFormQueryString representa uma URL para concatenar ao ponto de extremidade Outlook Web App para ler um item no Outlook Web App.
ms.openlocfilehash: 10035aa001c74926ae36e96e09b5b2995844cb68
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538468"
---
# <a name="webclientreadformquerystring"></a>WebClientReadFormQueryString

O **elemento WebClientReadFormQueryString** representa uma URL para concatenar ao ponto de extremidade Outlook Web App para ler um item no Outlook Web App. 
  
```XML
<WebClientReadFormQueryString/>
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
|[RemoveItem](removeitem.md) <br/> |Remove um item do Exchange store.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no Exchange store.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa uma cadeia de caracteres será necessário se esse elemento for usado.
  
## <a name="remarks"></a>Comentários

O identificador de item para uma URL Outlook Web App é o identificador EWS do item. Você pode codificar a URL do identificador de item EWS e aendá-lo à cadeia de caracteres de consulta para obter Outlook Web App URL de um item.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
### <a name="version-differences"></a>Diferenças de versão

As versões do Exchange começando com a versão principal 1 Exchange Server 5 e terminando com a com build 15.0.775.38 (CU3) e Exchange Online versão 15.00.0775.009 não retornam um fragmento de cadeia de caracteres de consulta correto no **elemento WebClientReadFormQueryString.** 
  
Em versões Exchange anteriores à versão principal 15, o identificador de item para Outlook Web App URLs é um identificador Outlook Web App. Se você estiver direcionando uma versão do Exchange versão principal 15, será preciso usar a operação [ConvertId](convertid-operation.md) para converter o identificador. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

