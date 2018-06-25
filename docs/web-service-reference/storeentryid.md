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
ms.openlocfilehash: dfd38e445ff0c5966116e984d712a45b6b1b8485
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825600"
---
# <a name="storeentryid"></a>StoreEntryId

O elemento **StoreEntryId** contém o identificador de repositório do Exchange de um item. 
  
```XML
<StoreEntryId/>
```

 **base64Binary**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Nome do elemento**|**Descrição**|
|:-----|:-----|
|[AcceptItem](acceptitem.md) <br/> |Representa uma resposta de aceitar a uma solicitação de reunião.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[Condições](conditions.md) <br/> |Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato no armazenamento do Exchange.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Representa uma resposta recusar a uma solicitação de reunião.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[Exceções](exceptions.md) <br/> |Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.  <br/> |
|[1.1](item.md) <br/> |Representa um item genérico do Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa o cancelamento da reunião no armazenamento do Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no armazenamento do Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no armazenamento do Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no armazenamento do Exchange.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem de email do Exchange.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Remove um item de armazenamento do Exchange.  <br/> |
|[Task](task.md) <br/> |Representa uma tarefa no armazenamento do Exchange.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Representa uma resposta provisoriamente aceita para uma solicitação de reunião.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto é uma cadeia de caracteres que representa o identificador do item de armazenamento.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
Este elemento foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).
  
## <a name="element-information"></a>Informações de elemento

||
|:-----|
|Namespace  <br/> |
|Nome do esquema  <br/> |
|Arquivo de validação  <br/> |
|Pode ser vazio  <br/> |
   

