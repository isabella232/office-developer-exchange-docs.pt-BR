---
title: MergedFreeBusy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MergedFreeBusy
api_type:
- schema
ms.assetid: ea45590d-476e-4b68-9fe8-ae392feadfea
description: O elemento MergedFreeBusy contém o fluxo de dados de disponibilidade mesclado.
ms.openlocfilehash: a1483449534f0d886e3c97a23d28c5d78f865042
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468723"
---
# <a name="mergedfreebusy"></a>MergedFreeBusy

O elemento **MergedFreeBusy** contém o fluxo de dados de disponibilidade mesclado. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[MergedFreeBusy](mergedfreebusy.md)
  
```xml
<MergedFreeBusy>...</MergedFreeBusy>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FreeBusyView](freebusyview.md) <br/> |Contém informações de disponibilidade para um usuário específico.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é fornecido pelo servidor se o valor para o elemento [FreeBusyViewType](freebusyviewtype.md) for um dos seguintes: 
  
- DetailedMerged
    
- FreeBusyMerged
    
- MergedOnly
    
O valor de texto é um fluxo de informações de disponibilidade. 
  
## <a name="remarks"></a>Comentários

O fluxo de dados fornecido por esse elemento é definido pelos elementos [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) e [TimeWindow](timewindow.md) . O elemento [TimeWindow](timewindow.md) define o intervalo de tempo consultado para disponibilidade. O elemento [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) define como o horário do elemento [TimeWindow](timewindow.md) é dividido em intervalos retornados no elemento **MergedFreeBusy** . Cada número no fluxo **MergedFreeBusy** representa um único intervalo definido pelo elemento [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) . A tabela a seguir lista os valores possíveis para um intervalo individual. 
  
|**Dígitos**|**Disponibilidade**|
|:-----|:-----|
|,0  <br/> |Disponível  <br/> |
|1   <br/> |Provisória  <br/> |
|duas  <br/> |Ocupado  <br/> |
|3D  <br/> |Ausência Temporária  <br/> |
|4   <br/> |Nenhum dado  <br/> |
   
Por exemplo, uma solicitação de dados de disponibilidade inclui um elemento [TimeWindow](timewindow.md) que representa quatro horas e um elemento [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) que representa 60 minutos. Se o calendário do usuário solicitado for OOF para os primeiros 60 minutos, ocupado pelos seguintes 90 minutos e não tiver sido agendado para o final de 90 minutos na janela de tempo, o fluxo **MergedFreeBusy** será 3220. Se um intervalo contiver mais de uma classificação de disponibilidade, o maior número será usado para classificar esse intervalo. 
  
O nível de detalhes fornecido por esse elemento depende das permissões concedidas ao solicitante.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserAvailability](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[Obtendo disponibilidade do usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

