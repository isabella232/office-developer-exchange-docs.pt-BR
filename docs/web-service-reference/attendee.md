---
title: Participante
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Attendee
api_type:
- schema
ms.assetid: 393c3d7e-7416-458a-b976-270b88eaaa03
description: O elemento participante representa participantes e recursos de uma reunião.
ms.openlocfilehash: f376e59b27017e0a9d27692cb1a4ae759cd1af0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457645"
---
# <a name="attendee"></a>Participante

O elemento **participante** representa participantes e recursos de uma reunião. 
  
```xml
<Attendee>
   <Mailbox/>
   <ResponseType/>
   <LastResponseTime/>
</Attendee>
```

 **Articipantetype**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Caixa de Correio](mailbox.md) <br/> |Identifica um endereço de email totalmente resolvido.  <br/> |
|[ResponseType](responsetype.md) <br/> |Representa o tipo de resposta de destinatário recebido para uma reunião. Essa propriedade só é relevante para o item de calendário do organizador da reunião.  <br/> |
|[LastResponseTime](lastresponsetime.md) <br/> |Representa a data e a hora da última resposta recebida.  <br/> |
|[ProposedStart](proposedstart-attendeetype.md) <br/> |Representa a hora de início proposta de um participante para uma reunião. <br/> |
|[ProposedEnd](proposedend-attendeetype.md) <br/> |Representa a hora de término proposta de um participante para uma reunião. <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RequiredAttendees](requiredattendees.md) <br/> |Representa participantes que são necessários para participar de uma reunião.  <br/> |
|[OptionalAttendees](optionalattendees.md) <br/> |Representa os participantes que não precisam participar de uma reunião.  <br/> |
|[Recursos](resources.md) <br/> |Representa um recurso agendado para uma reunião.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

