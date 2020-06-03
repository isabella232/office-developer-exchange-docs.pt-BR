---
title: RequestedView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequestedView
api_type:
- schema
ms.assetid: e2b4cf8c-5d43-4cd8-b86d-cc27a5d2f095
description: O elemento RequestedView define o tipo de informação do calendário que um cliente solicita.
ms.openlocfilehash: bc4f863841fc5a7d1d23f0bd4c7c2895d2593a2d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459157"
---
# <a name="requestedview"></a>RequestedView

O elemento **RequestedView** define o tipo de informação do calendário que um cliente solicita. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[FreeBusyViewOptions](freebusyviewoptions.md)
  
[RequestedView](requestedview.md)
  
```xml
<RequestedView>None or MergedOnly or FreeBusy or FreeBusyMerged or Detailed or DetailedMerged</RequestedView>
```

 **FreeBusyViewType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FreeBusyViewOptions](freebusyviewoptions.md) <br/> |Especifica o tipo de informações de disponibilidade retornadas na resposta.  <br/> Este é o XPath para este elemento:  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é obrigatório. A tabela a seguir lista os valores possíveis para este elemento.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|Nenhum  <br/> |Esse valor não é válido para solicitações. Esse valor é válido para respostas.  <br/> |
|MergedOnly  <br/> |Representa um fluxo de disponibilidade agregado. Em cenários de várias florestas nos quais o usuário de destino em uma floresta não tem um serviço de disponibilidade configurado, o serviço de disponibilidade do solicitante recupera as informações de disponibilidade do usuário de destino da pasta pública de disponibilidade. Como as pastas públicas só armazenam informações de disponibilidade no formato mesclado, o **MergedOnly** é a única informação disponível.  <br/> |
|FreeBusy  <br/> |Representa as informações de status herdadas: livre, ocupado, provisório e OOF. Isso também inclui as horas de início/término dos compromissos. Este modo de exibição é mais rico do que o modo de disponibilidade herdado, pois os horários de início e término da reunião individuais são fornecidos em vez de um fluxo de disponibilidade agregado.  <br/> |
|FreeBusyMerged  <br/> |Representa todas as propriedades no **FreeBusy** com um fluxo de informações de disponibilidade mescladas.  <br/> |
|Análise  <br/> |Representa as informações de status herdadas: livre, ocupado, provisório e OOF; os horários de início/término dos compromissos; e várias propriedades do compromisso, como assunto, local e importância. Este modo de exibição solicitado retornará a quantidade máxima de informações para as quais o usuário solicitante é privilegiado. Se as informações de disponibilidade mescladas somente estiverem disponíveis, como com a solicitação de informações para usuários em uma floresta do Microsoft Exchange Server 2003, **MergedOnly** será retornado. Caso contrário, **FreeBusy** ou **detailed** será retornado.  <br/> |
|DetailedMerged  <br/> |Representa todas as propriedades em **detalhes** com um fluxo de informações de disponibilidade mescladas. Se somente as informações de disponibilidade mescladas estiverem disponíveis, **MergedOnly** será retornado. Caso contrário, **FreeBusyMerged** ou **DetailedMerged** será retornado.  <br/> |
   
## <a name="remarks"></a>Comentários

O valor definido por este elemento é retornado com o elemento [FreeBusyViewType](freebusyviewtype.md) na resposta. 
  
A tabela a seguir mostra o que é retornado para os diferentes tipos de modo de exibição e a propriedade MAPI correspondente. Cada tipo de modo de exibição é criado com base no tipo de exibição anterior.
  
|**Tipo de exibição disponível/ocupado**|**Properties**|**Propriedade de calendário MAPI**|
|:-----|:-----|:-----|
|**MergedOnly** <br/> |MergedFreeBusyStream  <br/> ||
|**FreeBusy** <br/> |Status clássico  <br/> |PropTag (0x80860003)  <br/> |
|**FreeBusy** <br/> |Horário de trabalho  <br/> ||
|**FreeBusy** <br/> |Hora inicial  <br/> |PR_START_DATE  <br/> |
|**FreeBusy** <br/> |Hora final  <br/> |PR_END_DATE  <br/> |
|**FreeBusyMerged** <br/> |Status clássico  <br/> |PropTag (0x80860003)  <br/> |
|**FreeBusyMerged** <br/> |Horário de trabalho  <br/> ||
|**FreeBusyMerged** <br/> |Hora inicial  <br/> |PR_START_DATE  <br/> |
|**FreeBusyMerged** <br/> |Hora final  <br/> |PR_END_DATE  <br/> |
|**FreeBusyMerged** <br/> |MergedFreeBusyStream  <br/> ||
|**Análise** <br/> |Status clássico  <br/> |PropTag (0x80860003)  <br/> |
|**Análise** <br/> |Horário de trabalho  <br/> ||
|**Análise** <br/> |Hora inicial  <br/> |PR_START_DATE  <br/> |
|**Análise** <br/> |Hora final  <br/> |PR_END_DATE  <br/> |
|**Análise** <br/> |Assunto  <br/> |PR_SUBJECT  <br/> |
|**Análise** <br/> |Local  <br/> |PR_LOCATION  <br/> |
|**Análise** <br/> |Entry-ID (a menos que privado)  <br/> ||
|**Análise** <br/> |Sinalizador privado  <br/> ||
|**Análise** <br/> |Issatisfaçing  <br/> ||
|**Análise** <br/> |IsRecurring  <br/> ||
|**Análise** <br/> |IsException  <br/> ||
|**Análise** <br/> |ReminderSet  <br/> ||
|**DetailedMerged** <br/> |Status clássico  <br/> |PropTag (0x80860003)  <br/> |
|**DetailedMerged** <br/> |Horário de trabalho  <br/> ||
|**DetailedMerged** <br/> |Hora inicial  <br/> |PR_START_DATE  <br/> |
|**DetailedMerged** <br/> |Hora final  <br/> |PR_END_DATE  <br/> |
|**DetailedMerged** <br/> |Assunto  <br/> |PR_SUBJECT  <br/> |
|**DetailedMerged** <br/> |Local  <br/> |PR_LOCATION  <br/> |
|**DetailedMerged** <br/> |Entry-ID (a menos que privado)  <br/> ||
|**DetailedMerged** <br/> |Sinalizador privado  <br/> ||
|**DetailedMerged** <br/> |MergedFreeBusyStream  <br/> ||
|**DetailedMerged** <br/> |Issatisfaçing  <br/> ||
|**DetailedMerged** <br/> |IsRecurring  <br/> ||
|**DetailedMerged** <br/> |IsException  <br/> ||
|**DetailedMerged** <br/> |ReminderSet  <br/> ||
   
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserAvailability](getuseravailability-operation.md)


[Obtendo disponibilidade do usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

