---
title: IsOnlineMeeting
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsOnlineMeeting
api_type:
- schema
ms.assetid: c29df676-0f3a-4694-a42f-522c6d16872f
description: O elemento IsOnlineMeeting indica se a reunião online.
ms.openlocfilehash: 5a56b0b9828d6f6bec83fc0ad0f8f9579b471a72
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824061"
---
# <a name="isonlinemeeting"></a>IsOnlineMeeting

O elemento **IsOnlineMeeting** indica se a reunião online. 
  
```xml
<IsOnlineMeeting/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma reunião no armazenamento do Exchange.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
   
## <a name="text-value"></a>Text value

Se este elemento for usado, será necessário um valor de texto que representa um valor booleano. Um valor **true** indica que a reunião está online. Um valor **false** indica que a reunião não está online. 
  
## <a name="remarks"></a>Coment�rios

A propriedade IsOnlineMeeting é gravável de leitura para o item de calendário do organizador. Ele é somente leitura para solicitações de reunião e itens de calendário dos participantes.
  
O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o MicrosoftExchange 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

