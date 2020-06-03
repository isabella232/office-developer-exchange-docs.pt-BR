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
description: O elemento HasAttachments representa uma propriedade que é definida como true se um item tiver pelo menos um anexo visível ou se uma conversa contiver pelo menos um item que tenha um anexo. Essa propriedade é somente leitura.
ms.openlocfilehash: cc4e4ec0eac1c749723facc8cd780da41b0d8150
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462919"
---
# <a name="hasattachments"></a>HasAttachments

O elemento **HasAttachments** representa uma propriedade que é definida como **true** se um item tiver pelo menos um anexo visível ou se uma conversa contiver pelo menos um item que tenha um anexo. Essa propriedade é somente leitura. 
  
```XML
<HasAttachments/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[Condições](conditions.md) <br/> |Representa as condições que, ao serem atendidas, dispararão as ações de regra para essa regra.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato do Exchange.  <br/> |
|[Conversa (Conversatype)](conversation-conversationtype.md) <br/> |Representa uma única conversa.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[Exceções](exceptions.md) <br/> |Representa todas as condições de exceção de regra disponíveis para a regra de caixa de entrada.  <br/> |
|[Item](item.md) <br/> |Representa um item no repositório do Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no repositório do Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no repositório do Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no repositório do Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no repositório do Exchange.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem de email do Exchange.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no repositório do Exchange.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa um valor booliano é necessário. Um valor **true** significa que o item ou a conversa tem pelo menos um anexo visível. Um valor **false** significa que o item ou a conversa não tem nenhum anexo ou tem apenas anexos ocultos. 
  
## <a name="remarks"></a>Comentários

A propriedade **HasAttachments** é calculada a partir da propriedade Boolean **AllAttachmentsHidden** MAPI. Se um item não tiver um anexo, a propriedade **AllAttachmentsHidden** não existe. Se todos os anexos do item estiverem ocultos, a propriedade **AllAttachmentsHidden** será **true**. A propriedade **AllAttachmentsHidden** é **false** se tiver pelo menos um anexo e se pelo menos um dos anexos estiver visível. Use a propriedade MAPI **AllAttachmentsHidden** para pesquisar, agrupar e classificar itens. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
  
[Referência do EWS para Exchange](ews-reference-for-exchange.md)

