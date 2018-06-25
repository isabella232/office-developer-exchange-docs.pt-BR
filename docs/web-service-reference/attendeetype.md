---
title: AttendeeType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttendeeType
api_type:
- schema
ms.assetid: 048043a8-dbad-45a0-97c8-4cad63d8898b
description: O elemento AttendeeType representa o tipo de participante que é identificado no elemento de Email (EmailAddressType). Este elemento é usado nas solicitações para sugestões de reunião.
ms.openlocfilehash: a08532ed78296102ee252c1e0c40beee7ca8ea5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751230"
---
# <a name="attendeetype"></a>AttendeeType

O elemento **AttendeeType** representa o tipo de participante que é identificado no elemento de [Email (EmailAddressType)](email-emailaddresstype.md) . Este elemento é usado nas solicitações para sugestões de reunião. 
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
- [MailboxDataArray](mailboxdataarray.md)
  
- [MailboxData](mailboxdata.md)
  
- [AttendeeType](attendeetype.md)
  
```xml
<AttendeeType>Organizer or Required or Optional or Room or Resource</AttendeeType>
```

 **MeetingAttendeeType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MailboxData](mailboxdata.md) <br/> |Representa um usuário de caixa de correio individual e opções para o tipo de dados a serem retornadas sobre o usuário de caixa de correio.  <br/> Este é o XPath a este elemento:  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="text-value"></a>Text value

Um valor de texto é necessário para esse elemento. A tabela a seguir lista os valores possíveis para esse elemento.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|Organizador  <br/> |O usuário de caixa de correio e o participante que criou o item de calendário.  <br/> |
|Obrigatório  <br/> |Um usuário de caixa de correio que seja um participante necessário para a reunião.  <br/> |
|Opcional  <br/> |Um usuário de caixa de correio que um participante opcional para a reunião.  <br/> |
|Sala  <br/> |Uma entidade de caixa de correio que representa um recurso de sala usado para a reunião.  <br/> |
|Recurso  <br/> |Um recurso, como uma TV ou projetor que esteja agendado para ser usado na reunião.  <br/> |
   
## <a name="remarks"></a>Comentários

Este é um elemento necessário filho do elemento [MailboxData](mailboxdata.md) . Esse elemento pode ocorrer apenas uma vez no elemento [MailboxData](mailboxdata.md) . O esquema que descreve este elemento está localizado no diretório /EWS/ do computador que está executando o MicrosoftExchange Server 2007 que possui a função de servidor acesso para cliente instalada. 
  
> [!NOTE]
> O tipo de esquema AttendeeType é usado para representar um item de calendário de participantes. Não confunda esse elemento com elementos do tipo AttendeeType esquema. 
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [Obtenção de disponibilidade do usuário](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

