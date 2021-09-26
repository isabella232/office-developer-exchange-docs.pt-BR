---
title: StoreEntryId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f536e264-8c4d-4cc5-bab8-22a4fa38de39
description: O elemento StoreEntryId contém o Exchange de armazenamento de um item.
ms.openlocfilehash: 7ffd1d2ab6f68e772f27447b48fc305213aaed78
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544553"
---
# <a name="storeentryid"></a>StoreEntryId

O **elemento StoreEntryId** contém o Exchange de armazenamento de um item. 
  
```XML
<StoreEntryId/>
```

 **xs:base64Binary**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Nome do elemento**|**Descrição**|
|:-----|:-----|
|[AcceptItem](acceptitem.md) <br/> |Representa uma resposta de aceitação a uma solicitação de reunião.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um Exchange de calendário.  <br/> |
|[Condições](conditions.md) <br/> |Representa as condições que, quando cumpridas, dispararão as ações de regra para uma regra.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato no Exchange store.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Representa uma resposta de recusa a uma solicitação de reunião.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[Exceções](exceptions.md) <br/> |Representa todas as condições de exceção de regra disponíveis para uma regra de Caixa de Entrada.  <br/> |
|[Item](item.md) <br/> |Representa um item Exchange genérico.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no Exchange store.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no Exchange store.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no Exchange store.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no Exchange store.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma Exchange de email.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Remove um item do Exchange store.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no Exchange store.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Representa uma resposta aceita provisamente a uma solicitação de reunião.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto é uma cadeia de caracteres que representa o identificador de item do armazenamento.
  
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
   

