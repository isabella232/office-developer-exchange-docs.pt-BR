---
title: MergedFreeBusy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MergedFreeBusy
api_type:
- schema
ms.assetid: ea45590d-476e-4b68-9fe8-ae392feadfea
description: O elemento MergedFreeBusy contém o fluxo de dados livre/ocupado mesclado.
ms.openlocfilehash: db451d6b2e67313836771604fae57b14b6b3db10
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511027"
---
# <a name="mergedfreebusy"></a>MergedFreeBusy

O **elemento MergedFreeBusy** contém o fluxo de dados livre/ocupado mesclado. 
  
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
|[FreeBusyView](freebusyview.md) <br/> |Contém informações de disponibilidade para um usuário específico.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto será fornecido pelo servidor se o valor do [elemento FreeBusyViewType](freebusyviewtype.md) for um dos seguintes: 
  
- DetailedMerged
    
- FreeBusyMerged
    
- MergedOnly
    
O valor do texto é um fluxo de informações de livre/ocupado. 
  
## <a name="remarks"></a>Comentários

O fluxo de dados fornecidos por esse elemento é definido pelos elementos [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) e [TimeWindow.](timewindow.md) O [elemento TimeWindow](timewindow.md) define o intervalo de tempo consultado para disponibilidade. O [elemento MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) define como o tempo do [elemento TimeWindow](timewindow.md) é dividido em intervalos retornados no elemento **MergedFreeBusy.** Cada número no fluxo **MergedFreeBusy** representa um único intervalo definido pelo [elemento MergedFreeBusyIntervalInMinutes.](mergedfreebusyintervalinminutes.md) A tabela a seguir lista os valores possíveis para um intervalo individual. 
  
|**Dígito**|**Disponibilidade**|
|:-----|:-----|
|0  <br/> |Disponível  <br/> |
|1  <br/> |Tentativo  <br/> |
|2  <br/> |Ocupado  <br/> |
|3  <br/> |Ausência Temporária  <br/> |
|4   <br/> |Sem dados  <br/> |
   
Por exemplo, uma solicitação de dados de livre/ocupado inclui um elemento [TimeWindow](timewindow.md) que representa quatro horas e um [elemento MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) que representa 60 minutos. Se o calendário do usuário solicitado for OOF pelos primeiros 60 minutos, ocupado pelos 90 minutos seguintes e não agendado para os últimos 90 minutos na janela de tempo, o fluxo **MergedFreeBusy** será 3220. Se um intervalo contiver mais de uma classificação de disponibilidade, o número mais alto será usado para classificar esse intervalo. 
  
O nível de detalhes fornecido por esse elemento depende das permissões concedidas ao solicitante.
  
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

