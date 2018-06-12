---
title: FreeBusyViewType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyViewType
api_type:
- schema
ms.assetid: 7c7f82ba-fa52-4a3e-bec7-39d373c66fc7
description: O elemento FreeBusyViewType representa o tipo de informações de disponibilidade retornadas na resposta.
ms.openlocfilehash: fe965d062f72d99dff7148f4d00b12fd8c4e1366
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752385"
---
# <a name="freebusyviewtype"></a>FreeBusyViewType

O elemento **FreeBusyViewType** representa o tipo de informações de disponibilidade retornadas na resposta. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[FreeBusyViewType](freebusyviewtype.md)
  
```xml
<FreeBusyViewType>None or MergedOnly or FreeBusy or FreeBusyMerged or Detailed or DetailedMerged</FreeBusyViewType>
```

 **FreeBusyViewType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FreeBusyView](freebusyview.md) <br/> |Contém informações de disponibilidade para um usuário específico.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. A tabela a seguir lista os valores possíveis para esse elemento.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|None  <br/> |Este valor não é válido para solicitações. Esse valor é válido para respostas.  <br/> |
|MergedOnly  <br/> |Representa um fluxo de livre/ocupado agregado. Em cenários de entre florestas nas quais o usuário em uma floresta de destino não tem um serviço de disponibilidade configurado, o serviço de disponibilidade do solicitante recupera informações de disponibilidade do usuário de destino da pasta pública livre/ocupado. Como as pastas públicas somente armazenam informações de disponibilidade no formulário mesclado, **MergedOnly** são as informações de só está disponíveis.  <br/> |
|FreeBusy  <br/> |Representa as informações de status herdado: disponível, ocupado, provisório e ausência temporária. Isso também inclui as horas de início/término dos compromissos. Essa exibição é mais rica vez herdado de disponibilidade exibir porque individual reunião de início e término tempos são fornecidos em vez de um fluxo de livre/ocupado agregado.  <br/> |
|FreeBusyMerged  <br/> |Representa todas as propriedades na **FreeBusy** com um fluxo de informações de disponibilidade de livre/ocupado mesclado.  <br/> |
|Detalhada  <br/> |Representa as informações de status herdado: disponível, ocupado, provisório e OOF; os horários de início/término dos compromissos; e várias propriedades do compromisso como assunto, local e importância. Este modo de exibição solicitado retornará a quantidade máxima de informações para o qual o usuário solicitante é privilegiado. Se apenas informações de livre/ocupado mescladas estiverem disponíveis, como com solicitando informações para usuários em uma floresta do Microsoft Exchange Server 2003, **MergedOnly** será retornado. Caso contrário, **FreeBusy** ou **detalhado** será retornado.  <br/> Se **Detailed** for especificado para uma lista de distribuição, as informações de disponibilidade para os membros da lista são mescladas e **MergedOnly** é retornado.  <br/> |
|DetailedMerged  <br/> |Representa todas as propriedades na **Detailed** com um fluxo de informações de disponibilidade de livre/ocupado mesclado. Se houver apenas informações de livre/ocupado mescladas disponíveis, por exemplo, se a caixa de correio existir em um computador executando o Exchange 2003, **MergedOnly** será retornado. Caso contrário, **FreeBusyMerged** ou **DetailedMerged** serão retornados.  <br/> |
   
## <a name="remarks"></a>Coment�rios

Esse elemento é necessário se o elemento [FreeBusyView](freebusyview.md) é usado. O tipo de informações de disponibilidade retornadas é designado no elemento [RequestedView](requestedview.md) . O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente. 
  
A tabela a seguir mostra o que é retornado para os tipos de exibição diferentes e a propriedade MAPI correspondente. Cada tipo de exibição se baseia no tipo de visualização anterior.
  
|**FreeBusyViewType**|**Properties**|**Propriedade de Calendário MAPI**|
|:-----|:-----|:-----|
|**MergedOnly** <br/> |MergedFreeBusyStream  <br/> ||
|**FreeBusy** <br/> |Status clássico  <br/> |PropTag (0x80860003)  <br/> |
|**FreeBusy** <br/> |Horário de trabalho  <br/> ||
|**FreeBusy** <br/> |Hora de início  <br/> |PR_START_DATE  <br/> |
|**FreeBusy** <br/> |Hora de término  <br/> |PR_END_DATE  <br/> |
|**FreeBusyMerged** <br/> |Status clássico  <br/> |PropTag (0x80860003)  <br/> |
|**FreeBusyMerged** <br/> |Horário de trabalho  <br/> ||
|**FreeBusyMerged** <br/> |Hora de início  <br/> |PR_START_DATE  <br/> |
|**FreeBusyMerged** <br/> |Hora de término  <br/> |PR_END_DATE  <br/> |
|**FreeBusyMerged** <br/> |MergedFreeBusyStream  <br/> ||
|**Detalhadas** <br/> |Status clássico  <br/> |PropTag (0x80860003)  <br/> |
|**Detalhadas** <br/> |Horário de trabalho  <br/> ||
|**Detalhadas** <br/> |Hora de início  <br/> |PR_START_DATE  <br/> |
|**Detalhadas** <br/> |Hora de término  <br/> |PR_END_DATE  <br/> |
|**Detalhadas** <br/> |Assunto  <br/> |PR_SUBJECT  <br/> |
|**Detalhadas** <br/> |Local  <br/> |PR_LOCATION  <br/> |
|**Detalhadas** <br/> |Entrada-Id(unless private)  <br/> ||
|**Detalhadas** <br/> |Sinalizador particular  <br/> ||
|**Detalhadas** <br/> |IsMeeting  <br/> ||
|**Detalhadas** <br/> |IsRecurring  <br/> ||
|**Detalhadas** <br/> |IsException  <br/> ||
|**Detalhadas** <br/> |IsReminderSet  <br/> ||
|**Detalhadas** <br/> |Mensagem de ausência temporária (se solicitado)  <br/> ||
|**DetailedMerged** <br/> |Status clássico  <br/> |PropTag (0x80860003)  <br/> |
|**DetailedMerged** <br/> |Horário de trabalho  <br/> ||
|**DetailedMerged** <br/> |Hora de início  <br/> |PR_START_DATE  <br/> |
|**DetailedMerged** <br/> |Hora de término  <br/> |PR_END_DATE  <br/> |
|**DetailedMerged** <br/> |Assunto  <br/> |PR_SUBJECT  <br/> |
|**DetailedMerged** <br/> |Local  <br/> |PR_LOCATION  <br/> |
|**DetailedMerged** <br/> |Entrada-Id(unless private)  <br/> ||
|**DetailedMerged** <br/> |Sinalizador particular  <br/> ||
|**DetailedMerged** <br/> |MergedFreeBusyStream  <br/> ||
|**DetailedMerged** <br/> |IsMeeting  <br/> ||
|**DetailedMerged** <br/> |IsRecurring  <br/> ||
|**DetailedMerged** <br/> |IsException  <br/> ||
|**DetailedMerged** <br/> |IsReminderSet  <br/> ||
   
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação GetUserAvailability](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[Obtenção de disponibilidade do usuário](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

