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
description: O elemento MergedFreeBusy contém mesclado livre/ocupado fluxo de dados.
ms.openlocfilehash: 542b9fae0c36b0236bd806e8a9117753968e812c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824449"
---
# <a name="mergedfreebusy"></a>MergedFreeBusy

O elemento **MergedFreeBusy** contém mesclado livre/ocupado fluxo de dados. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[MergedFreeBusy](mergedfreebusy.md)
  
```xml
<MergedFreeBusy>...</MergedFreeBusy>
```

 **cadeia de caracteres**
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

Um valor de texto for fornecido pelo servidor se o valor para o elemento [FreeBusyViewType](freebusyviewtype.md) for um destes procedimentos: 
  
- DetailedMerged
    
- FreeBusyMerged
    
- MergedOnly
    
O valor de texto é um fluxo de informações de livre/ocupado. 
  
## <a name="remarks"></a>Coment�rios

Fluxo de dados fornecidos por esse elemento é definido pelos elementos [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) e [TimeWindow](timewindow.md) . O elemento de [TimeWindow](timewindow.md) define o intervalo de tempo consultado para disponibilidade. O elemento de [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) define como o tempo do elemento [TimeWindow](timewindow.md) é dividido em intervalos retornados no elemento **MergedFreeBusy** . Cada número no stream **MergedFreeBusy** representa um único intervalo definido pelo elemento [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) . A tabela a seguir lista os valores possíveis para um intervalo individual. 
  
|**Dígito**|**Disponibilidade**|
|:-----|:-----|
|0  <br/> |Disponível  <br/> |
|1  <br/> |Provisório  <br/> |
|2  <br/> |Ocupado  <br/> |
|3  <br/> |Out of Office (OOF)  <br/> |
|4  <br/> |Nenhum dado  <br/> |
   
Por exemplo, uma solicitação de dados do tipo disponível/ocupado inclui um elemento [TimeWindow](timewindow.md) que representa as quatro horas e um elemento [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) que representa 60 minutos. Se calendário do usuário solicitado OOF nos primeiros 60 minutos, ocupada pelos seguintes 90 minutos e não agendada para os finais 90 minutos na janela de tempo, o fluxo de **MergedFreeBusy** será 3220. Se um intervalo contiver mais de uma classificação de disponibilidade, o maior número é usado para classificar esse intervalo. 
  
O nível de detalhes fornecidos por esse elemento depende as permissões concedidas para o solicitante.
  
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

