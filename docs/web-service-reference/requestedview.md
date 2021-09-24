---
title: RequestedView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RequestedView
api_type:
- schema
ms.assetid: e2b4cf8c-5d43-4cd8-b86d-cc27a5d2f095
description: O elemento RequestedView define o tipo de informação de calendário que um cliente solicita.
ms.openlocfilehash: 350922a7fef90c26ace0ef8be07ebb866d304eb3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509473"
---
# <a name="requestedview"></a>RequestedView

O **elemento RequestedView** define o tipo de informação de calendário que um cliente solicita. 
  
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
|[FreeBusyViewOptions](freebusyviewoptions.md) <br/> |Especifica o tipo de informação de ocupado/livre retornada na resposta.  <br/> Veja a seguir o XPath para este elemento:  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. A tabela a seguir lista os valores possíveis para esse elemento.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|Nenhum  <br/> |Esse valor não é válido para solicitações. Esse valor é válido para respostas.  <br/> |
|MergedOnly  <br/> |Representa um fluxo de livre/ocupado agregado. Em cenários entre florestas em que o usuário de destino em uma floresta não tem um serviço de Disponibilidade configurado, o serviço de disponibilidade do solicitante recupera as informações de disponibilidade do usuário de destino da pasta pública de disponibilidade. Como as pastas públicas armazenam apenas informações de disponibilidade no formulário mesclado, **MergedOnly** é a única informação disponível.  <br/> |
|FreeBusy  <br/> |Representa as informações de status herdados: livre, ocupado, provisório e OOF. Isso também inclui os horários de início/término dos compromissos. Essa exibição é mais rica do que a exibição de livre/ocupado herdado porque os horários de início e fim de reunião individuais são fornecidos em vez de um fluxo de livre/ocupado agregado.  <br/> |
|FreeBusyMerged  <br/> |Representa todas as propriedades **no FreeBusy** com um fluxo de informações mescladas de livre/ocupado.  <br/> |
|Detalhado  <br/> |Representa as informações de status herdados: livre, ocupado, provisório e OOF; os horários de início/término dos compromissos; e várias propriedades do compromisso, como assunto, local e importância. Essa exibição solicitada retornará a quantidade máxima de informações para as quais o usuário solicitando é privilegiado. Se somente as informações de disponibilidade mescladas estão disponíveis, como com a solicitação de informações para usuários em uma floresta Microsoft Exchange Server 2003, **MergedOnly** será retornado. Caso contrário, **FreeBusy** **ou Detailed** serão retornados.  <br/> |
|DetailedMerged  <br/> |Representa todas as propriedades **em Detalhado com** um fluxo de informações mescladas de livre/ocupado. Se somente as informações de disponibilidade mescladas estão disponíveis, **MergedOnly** será retornado. Caso contrário, **FreeBusyMerged** ou **DetailedMerged** serão retornados.  <br/> |
   
## <a name="remarks"></a>Comentários

O valor definido por esse elemento é retornado com o [elemento FreeBusyViewType](freebusyviewtype.md) na resposta. 
  
A tabela a seguir mostra o que é retornado para os diferentes tipos de exibição e a propriedade MAPI correspondente. Cada tipo de exibição é construído com base no tipo de exibição anterior.
  
|**Tipo de exibição de ocupado/livre**|**Propriedades**|**Propriedade MAPI Calendar**|
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
|**Detalhado** <br/> |Status clássico  <br/> |PropTag (0x80860003)  <br/> |
|**Detalhado** <br/> |Horário de trabalho  <br/> ||
|**Detalhado** <br/> |Hora inicial  <br/> |PR_START_DATE  <br/> |
|**Detalhado** <br/> |Hora final  <br/> |PR_END_DATE  <br/> |
|**Detalhado** <br/> |Assunto  <br/> |PR_SUBJECT  <br/> |
|**Detalhado** <br/> |Local  <br/> |PR_LOCATION  <br/> |
|**Detalhado** <br/> |Id de entrada(a menos que particular)  <br/> ||
|**Detalhado** <br/> |Sinalizador Particular  <br/> ||
|**Detalhado** <br/> |IsMeeting  <br/> ||
|**Detalhado** <br/> |IsRecurring  <br/> ||
|**Detalhado** <br/> |IsException  <br/> ||
|**Detalhado** <br/> |IsReminderSet  <br/> ||
|**DetailedMerged** <br/> |Status clássico  <br/> |PropTag (0x80860003)  <br/> |
|**DetailedMerged** <br/> |Horário de trabalho  <br/> ||
|**DetailedMerged** <br/> |Hora inicial  <br/> |PR_START_DATE  <br/> |
|**DetailedMerged** <br/> |Hora final  <br/> |PR_END_DATE  <br/> |
|**DetailedMerged** <br/> |Assunto  <br/> |PR_SUBJECT  <br/> |
|**DetailedMerged** <br/> |Local  <br/> |PR_LOCATION  <br/> |
|**DetailedMerged** <br/> |Id de entrada(a menos que particular)  <br/> ||
|**DetailedMerged** <br/> |Sinalizador Particular  <br/> ||
|**DetailedMerged** <br/> |MergedFreeBusyStream  <br/> ||
|**DetailedMerged** <br/> |IsMeeting  <br/> ||
|**DetailedMerged** <br/> |IsRecurring  <br/> ||
|**DetailedMerged** <br/> |IsException  <br/> ||
|**DetailedMerged** <br/> |IsReminderSet  <br/> ||
   
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserAvailability](getuseravailability-operation.md)


[Obter Disponibilidade do Usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

