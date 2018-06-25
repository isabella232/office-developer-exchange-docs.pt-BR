---
title: FreeBusyView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyView
api_type:
- schema
ms.assetid: cb18434f-5f41-4e05-a5ce-d921b2721a8c
description: O elemento FreeBusyView contém informações de disponibilidade para um usuário específico.
ms.openlocfilehash: d0d603f18642a94e841a1a6bb8e8849aa6b5b273
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752370"
---
# <a name="freebusyview"></a>FreeBusyView

O elemento **FreeBusyView** contém informações de disponibilidade para um usuário específico. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
```xml
<FreeBusyView>
   <FreeBusyViewType>...</FreeBusyViewType>
   <MergedFreeBusy>...</MergedFreeBusy>
   <CalendarEventArray>...</CalendarEventArray>
   <WorkingHours>...</WorkingHours>
</FreeBusyView>
```

 **FreeBusyView**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FreeBusyViewType](freebusyviewtype.md) <br/> |Representa o tipo de informações de livre/ocupado solicitadas retornados na resposta.  <br/> |
|[MergedFreeBusy](mergedfreebusy.md) <br/> |Contém mesclado livre/ocupado fluxo de dados.  <br/> |
|[CalendarEventArray](calendareventarray.md) <br/> |Contém um conjunto de ocorrências de item de calendário exclusivo que representam a disponibilidade do usuário solicitado.  <br/> |
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |Representa as configurações de fuso horário e o horário de trabalho para o usuário de caixa de correio solicitada.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FreeBusyResponse](freebusyresponse.md) <br/> |Contém as informações de disponibilidade para um usuário de caixa de correio única.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse` <br/> |
   
## <a name="remarks"></a>Comentários

Todos os elementos filhos são listados na sequência em que ocorrem. O nível de detalhes fornecidos por esse elemento depende as permissões concedidas para o solicitante.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
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

