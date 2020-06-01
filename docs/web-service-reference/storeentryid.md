---
title: StoreEntryId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f536e264-8c4d-4cc5-bab8-22a4fa38de39
description: O elemento StoreEntryId contém o identificador de repositório do Exchange de um item.
ms.openlocfilehash: 669ea937da6c08b50877c24aeb450fe975326247
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465153"
---
# <a name="storeentryid"></a>StoreEntryId

O elemento **StoreEntryId** contém o identificador de repositório do Exchange de um item. 
  
```XML
<StoreEntryId/>
```

 **xs: base64Binary**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Nome do elemento**|**Descrição**|
|:-----|:-----|
|[AcceptItem](acceptitem.md) <br/> |Representa uma resposta de aceitação para uma solicitação de reunião.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[Condições](conditions.md) <br/> |Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato no repositório do Exchange.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Representa uma resposta de recusa a uma solicitação de reunião.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[Exceções](exceptions.md) <br/> |Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.  <br/> |
|[Item](item.md) <br/> |Representa um item genérico do Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no repositório do Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no repositório do Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no repositório do Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no repositório do Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem de email do Exchange.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Remove um item do repositório do Exchange.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no repositório do Exchange.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Representa uma resposta provisoriamente aceita a uma solicitação de reunião.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto é uma cadeia de caracteres que representa o identificador de item de armazenamento.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
Este elemento foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).
  
## <a name="element-information"></a>Elemento de informações

||
|:-----|
|Namespace  <br/> |
|Nome do esquema  <br/> |
|Arquivo de validação  <br/> |
|Pode ser vazio  <br/> |
   

