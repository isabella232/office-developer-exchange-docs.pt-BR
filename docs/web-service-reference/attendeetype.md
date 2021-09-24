---
title: AttendeeType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AttendeeType
api_type:
- schema
ms.assetid: 048043a8-dbad-45a0-97c8-4cad63d8898b
description: O elemento AttendeeType representa o tipo de participante identificado no elemento Email (EmailAddressType). Esse elemento é usado em solicitações para sugestões de reunião.
ms.openlocfilehash: 5bcec50fe6cccc3df48ca9615dbd0d9418211b4b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533931"
---
# <a name="attendeetype"></a>AttendeeType

O **elemento AttendeeType** representa o tipo de participante identificado no [elemento Email (EmailAddressType).](email-emailaddresstype.md) Esse elemento é usado em solicitações para sugestões de reunião. 
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
- [MailboxDataArray](mailboxdataarray.md)
  
- [MailboxData](mailboxdata.md)
  
- [AttendeeType](attendeetype.md)
  
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
|[MailboxData](mailboxdata.md) <br/> |Representa um usuário de caixa de correio individual e opções para o tipo de dados a serem retornados sobre o usuário da caixa de correio.  <br/> Veja a seguir o XPath para este elemento:  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário para esse elemento. A tabela a seguir lista os valores possíveis para esse elemento.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|Organizer  <br/> |O usuário da caixa de correio e o participante que criou o item de calendário.  <br/> |
|Obrigatório  <br/> |Um usuário de caixa de correio que é um participante obrigatório para a reunião.  <br/> |
|Opcional  <br/> |Um usuário de caixa de correio que é um participante opcional da reunião.  <br/> |
|Room  <br/> |Uma entidade de caixa de correio que representa um recurso de sala usado para a reunião.  <br/> |
|Recurso  <br/> |Um recurso como uma TV ou projetor agendado para uso na reunião.  <br/> |
   
## <a name="remarks"></a>Comentários

Esse elemento é um elemento filho necessário do elemento [MailboxData.](mailboxdata.md) Esse elemento só pode ocorrer uma vez no [elemento MailboxData.](mailboxdata.md) O esquema que descreve esse elemento está localizado no diretório /EWS/do computador que está executando o MicrosoftExchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada. 
  
> [!NOTE]
> O tipo de esquema AttendeeType é usado para representar participantes a um item de calendário. Não confunda esse elemento com elementos do tipo de esquema AttendeeType. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [Obter Disponibilidade do Usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

