---
title: Articipantetype
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
description: O elemento attendetype representa o tipo de participante identificado no elemento email (EmailAddresstype). Este elemento é usado em solicitações de sugestões de reunião.
ms.openlocfilehash: 104b9f38cc891310ecb47c0b47837a912ced6ab7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462294"
---
# <a name="attendeetype"></a>Articipantetype

O elemento **Attendetype** representa o tipo de participante identificado no elemento [email (EmailAddressType)](email-emailaddresstype.md) . Este elemento é usado em solicitações de sugestões de reunião. 
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
- [MailboxDataArray](mailboxdataarray.md)
  
- [MailboxData](mailboxdata.md)
  
- [Articipantetype](attendeetype.md)
  
```xml
<AttendeeType>Organizer or Required or Optional or Room or Resource</AttendeeType>
```

 **MeetingAttendeeType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MailboxData](mailboxdata.md) <br/> |Representa um usuário de caixa de correio individual e opções para o tipo de dados a ser retornado sobre o usuário da caixa de correio.  <br/> Este é o XPath para este elemento:  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário para este elemento. A tabela a seguir lista os valores possíveis para este elemento.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|Organizador  <br/> |O usuário de caixa de correio e participante que criou o item de calendário.  <br/> |
|Obrigatório  <br/> |Um usuário de caixa de correio que é um participante necessário para a reunião.  <br/> |
|Opcional  <br/> |Um usuário de caixa de correio que é um participante opcional da reunião.  <br/> |
|Sala  <br/> |Uma entidade de caixa de correio que representa um recurso de sala usado para a reunião.  <br/> |
|Resource  <br/> |Um recurso como uma TV ou um projetor agendado para uso na reunião.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento é um elemento filho obrigatório do elemento [MailboxData](mailboxdata.md) . Este elemento só pode ocorrer uma vez no elemento [MailboxData](mailboxdata.md) . O esquema que descreve este elemento está localizado no diretório/EWS/do computador que está executando o MicrosoftExchange Server 2007 que tem a função de servidor de acesso para Cliente instalada. 
  
> [!NOTE]
> O tipo de esquema attendetype é usado para representar participantes para um item de calendário. Não confunda este elemento com elementos do tipo de esquema attendetype. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [Obtendo disponibilidade do usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

