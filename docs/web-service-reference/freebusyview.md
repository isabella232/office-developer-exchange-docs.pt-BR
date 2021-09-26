---
title: FreeBusyView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FreeBusyView
api_type:
- schema
ms.assetid: cb18434f-5f41-4e05-a5ce-d921b2721a8c
description: O elemento FreeBusyView contém informações de disponibilidade para um usuário específico.
ms.openlocfilehash: c662e8a44118f61b4c8be642d9ac862051c3a15d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546410"
---
# <a name="freebusyview"></a>FreeBusyView

O **elemento FreeBusyView** contém informações de disponibilidade para um usuário específico. 
  
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
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FreeBusyViewType](freebusyviewtype.md) <br/> |Representa o tipo de informação de livre/ocupado solicitada retornada na resposta.  <br/> |
|[MergedFreeBusy](mergedfreebusy.md) <br/> |Contém o fluxo de dados livre/ocupado mesclado.  <br/> |
|[CalendarEventArray](calendareventarray.md) <br/> |Contém um conjunto de ocorrências de item de calendário exclusivas que representam a disponibilidade do usuário solicitado.  <br/> |
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |Representa as configurações de fuso horário e o horário de trabalho para o usuário de caixa de correio solicitado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FreeBusyResponse](freebusyresponse.md) <br/> |Contém as informações de ocupado/livre para um único usuário de caixa de correio.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse` <br/> |
   
## <a name="remarks"></a>Comentários

Todos os elementos filho são listados na sequência em que ocorrem. O nível de detalhes fornecido por esse elemento depende das permissões concedidas ao solicitante.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
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

