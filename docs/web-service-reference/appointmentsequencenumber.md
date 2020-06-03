---
title: AppointmentSequenceNumber
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppointmentSequenceNumber
api_type:
- schema
ms.assetid: eb4c48bd-f905-48dc-ae16-53a080b9b025
description: O elemento AppointmentSequenceNumber especifica o número de sequência de uma versão de um compromisso.
ms.openlocfilehash: daeea7a656c59923bcb6f2850539c7869d6eb181
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461657"
---
# <a name="appointmentsequencenumber"></a>AppointmentSequenceNumber

O elemento **AppointmentSequenceNumber** especifica o número de sequência de uma versão de um compromisso. 
  
```xml
<AppointmentSequenceNumber/>
```

 **int**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no repositório do Exchange.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa um número de versão.
  
## <a name="remarks"></a>Comentários

Esse valor é atualizado quando o compromisso é atualizado com as novas informações. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

