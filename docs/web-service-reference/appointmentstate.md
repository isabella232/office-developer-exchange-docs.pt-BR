---
title: AppointmentState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppointmentState
api_type:
- schema
ms.assetid: ab3f5d04-ace1-4a15-9107-cefa6c41abc7
description: O elemento AppointmentState Especifica o status do compromisso.
ms.openlocfilehash: 05e92a3fea10a84518b0680c425011a91bc43d93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751190"
---
# <a name="appointmentstate"></a>AppointmentState

O elemento **AppointmentState** Especifica o status do compromisso. 
  
```XML
<AppointmentState/>
```

 **int**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma reunião no armazenamento do Exchange.  <br/> |
   
## <a name="text-value"></a>Text value

Esse elemento contém um valor de texto que representa o conjunto de bits. Isso é no formulário inteiro. Este elemento é somente leitura. Ele só será retornado em uma resposta.
  
## <a name="remarks"></a>Coment�rios

O valor de inteiro retornado representa a máscara de bits de estado do compromisso. A tabela a seguir descreve cada bit.
  
|**Name**|**Bit**|**Descrição**|
|:-----|:-----|:-----|
|None  <br/> |0x0000  <br/> |Nenhum sinalizador foram definidos. Isso é usado apenas para um compromisso que não inclui os participantes.  <br/> |
|Reunião  <br/> |0x0001  <br/> |Este compromisso é uma reunião.  <br/> |
|Received  <br/> |0x0002  <br/> |Este compromisso foi recebido.  <br/> |
|Cancelado  <br/> |0x0004  <br/> |Este compromisso foi cancelado.  <br/> |
   
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

