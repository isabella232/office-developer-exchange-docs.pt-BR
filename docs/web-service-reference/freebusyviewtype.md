---
title: FreeBusyViewType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FreeBusyViewType
api_type:
- schema
ms.assetid: 7c7f82ba-fa52-4a3e-bec7-39d373c66fc7
description: O elemento FreeBusyViewType representa o tipo de informação de ocupado/livre retornada na resposta.
ms.openlocfilehash: 6eec490b39ccb9c02e7a16c8da7cfdd57f9b92c5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509921"
---
# <a name="freebusyviewtype"></a>FreeBusyViewType

O **elemento FreeBusyViewType** representa o tipo de informação de ocupado/livre retornada na resposta. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[FreeBusyViewType](freebusyviewtype.md)
  
```xml
<FreeBusyViewType>None or MergedOnly or FreeBusy or FreeBusyMerged or Detailed or DetailedMerged</FreeBusyViewType>
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
|[FreeBusyView](freebusyview.md) <br/> |Contém informações de disponibilidade para um usuário específico.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. A tabela a seguir lista os valores possíveis para esse elemento.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|Nenhum  <br/> |Esse valor não é válido para solicitações. Esse valor é válido para respostas.  <br/> |
|MergedOnly  <br/> |Representa um fluxo de livre/ocupado agregado. Em cenários entre florestas em que o usuário de destino em uma floresta não tem um serviço de Disponibilidade configurado, o serviço de disponibilidade do solicitante recupera as informações de disponibilidade do usuário de destino da pasta pública de disponibilidade. Como as pastas públicas armazenam apenas informações de disponibilidade no formulário mesclado, **MergedOnly** é a única informação disponível.  <br/> |
|FreeBusy  <br/> |Representa as informações de status herdados: livre, ocupado, provisório e OOF. Isso também inclui os horários de início/término dos compromissos. Essa exibição é mais rica do que a exibição de livre/ocupado herdado porque os horários de início e fim de reunião individuais são fornecidos em vez de um fluxo de livre/ocupado agregado.  <br/> |
|FreeBusyMerged  <br/> |Representa todas as propriedades no **FreeBusy** com um fluxo de informações de disponibilidade livre/ocupado mescladas.  <br/> |
|Detalhado  <br/> |Representa as informações de status herdados: livre, ocupado, provisório e OOF; os horários de início/término dos compromissos; e várias propriedades do compromisso, como assunto, local e importância. Essa exibição solicitada retornará a quantidade máxima de informações para as quais o usuário solicitando é privilegiado. Se somente as informações de disponibilidade mescladas estão disponíveis, como com a solicitação de informações para usuários em uma floresta Microsoft Exchange Server 2003, **MergedOnly** será retornado. Caso contrário, **FreeBusy** **ou Detailed** serão retornados.  <br/> Se **Detailed** for especificado para uma lista de distribuição, as informações de livre/ocupado para os membros da lista são mescladas e **MergedOnly** é retornada.  <br/> |
|DetailedMerged  <br/> |Representa todas as propriedades **em Detalhado com** um fluxo de informações de disponibilidade livre/ocupado mescladas. Se apenas as informações de disponibilidade mescladas estão disponíveis, por exemplo, se a caixa de correio existir em um computador executando Exchange 2003, **MergedOnly** será retornado. Caso contrário, **FreeBusyMerged** ou **DetailedMerged** serão retornados.  <br/> |
   
## <a name="remarks"></a>Comentários

Esse elemento será necessário se o [elemento FreeBusyView](freebusyview.md) for usado. O tipo de informação de ocupado/livre retornado é designado no [elemento RequestedView.](requestedview.md) O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente. 
  
A tabela a seguir mostra o que é retornado para os diferentes tipos de exibição e a propriedade MAPI correspondente. Cada tipo de exibição é construído com base no tipo de exibição anterior.
  
|**FreeBusyViewType**|**Propriedades**|**Propriedade MAPI Calendar**|
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
|**Detalhado** <br/> |Sem Office Mensagem (se solicitado)  <br/> ||
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
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[Obter Disponibilidade do Usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

