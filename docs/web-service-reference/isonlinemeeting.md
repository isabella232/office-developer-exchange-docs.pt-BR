---
title: IsOnlineMeeting
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsOnlineMeeting
api_type:
- schema
ms.assetid: c29df676-0f3a-4694-a42f-522c6d16872f
description: O elemento IsOnlineMeeting indica se a reunião está online.
ms.openlocfilehash: 3521cf82f2b6b2b2514b82478fc4e1e5c6edb563
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514512"
---
# <a name="isonlinemeeting"></a>IsOnlineMeeting

O **elemento IsOnlineMeeting** indica se a reunião está online. 
  
```xml
<IsOnlineMeeting/>
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
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma reunião no Exchange store.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um Exchange de calendário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa um valor Boolean é necessário se esse elemento for usado. Um valor **verdadeiro** indica que a reunião está online. Um valor **false** indica que a reunião não está online. 
  
## <a name="remarks"></a>Comentários

A propriedade IsOnlineMeeting pode ser lida para o item de calendário do organizador. Ele é somente leitura para solicitações de reunião e itens de calendário dos participantes.
  
O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

