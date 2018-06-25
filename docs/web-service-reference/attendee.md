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
description: O elemento Attendee representa participantes e recursos para uma reunião.
ms.openlocfilehash: 60cb0839c2f6de69b833c11f4594d40c14cd8887
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751225"
---
# <a name="attendee"></a>Participante

O elemento **Attendee** representa participantes e recursos para uma reunião. 
  
```xml
<Attendee>
   <Mailbox/>
   <ResponseType/>
   <LastResponseTime/>
</Attendee>
```

 **AttendeeType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Caixa de correio](mailbox.md) <br/> |Identifica um endereço de email totalmente resolvido.  <br/> |
|[ResponseType](responsetype.md) <br/> |Representa o tipo de destinatário resposta recebida para uma reunião. Essa propriedade só é relevante para o item de calendário do organizador da reunião.  <br/> |
|[LastResponseTime](lastresponsetime.md) <br/> |Representa a data e hora da resposta mais recente que é recebida.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RequiredAttendees](requiredattendees.md) <br/> |Representa os participantes necessários para participar de uma reunião.  <br/> |
|[OptionalAttendees](optionalattendees.md) <br/> |Representa a participantes que não são necessárias para participar de uma reunião.  <br/> |
|[Recursos](resources.md) <br/> |Representa um recurso agendado para uma reunião.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

