---
title: HasAttachments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HasAttachments
api_type:
- schema
ms.assetid: 538b7a85-11d7-4daa-8458-09b540760e8b
description: O elemento HasAttachments representa uma propriedade que é definida como true se um item tem pelo menos um anexo visível ou se uma conversa contém pelo menos um item que tenha um anexo. Esta propriedade é somente leitura.
ms.openlocfilehash: e76e0ecbb357396540f0d1649cf5062edfb18660
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823801"
---
# <a name="hasattachments"></a>HasAttachments

O elemento **HasAttachments** representa uma propriedade que é definida como **true** se um item tem pelo menos um anexo visível ou se uma conversa contém pelo menos um item que tenha um anexo. Esta propriedade é somente leitura. 
  
```XML
<HasAttachments/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[Condições](conditions.md) <br/> |Representa as condições que, quando atendida, irá disparar as ações de regra para essa regra.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato do Exchange.  <br/> |
|[Conversa (ConversationType)](conversation-conversationtype.md) <br/> |Representa uma única conversa.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[Exceções](exceptions.md) <br/> |Representa todas as condições de exceção de regra disponíveis para a regra de caixa de entrada.  <br/> |
|[1.1](item.md) <br/> |Representa um item no armazenamento do Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa o cancelamento da reunião no armazenamento do Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no armazenamento do Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no armazenamento do Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no armazenamento do Exchange.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem de email do Exchange.  <br/> |
|[Task](task.md) <br/> |Representa uma tarefa no armazenamento do Exchange.  <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto que representa um valor booleano. Um valor **true** significa que o item ou conversa tem pelo menos um anexo visível. Um valor **false** significa que o item ou conversa sem anexos ou somente tem oculto anexos. 
  
## <a name="remarks"></a>Coment�rios

A propriedade **HasAttachments** é calculada da propriedade MAPI de **AllAttachmentsHidden** booleano. Se um item não tiver um anexo, a propriedade **AllAttachmentsHidden** não existe. Se todos os anexos no item estiver oculto, a propriedade **AllAttachmentsHidden** é **true**. A propriedade **AllAttachmentsHidden** for **Falso** , se ele tiver sido definido pelo menos um anexo e pelo menos um dos anexos está visível. Use a propriedade MAPI **AllAttachmentsHidden** para pesquisa, agrupar e classificar itens. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
  
[Referência do EWS para Exchange](ews-reference-for-exchange.md)

