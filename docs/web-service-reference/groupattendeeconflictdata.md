---
title: GroupAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupAttendeeConflictData
api_type:
- schema
ms.assetid: fd8bf19a-298b-4135-93e8-ead3db7e1142
description: O elemento GroupAttendeeConflictData contém informações de conflito agregadas sobre o número de usuários que estão disponíveis, o número de usuários que possuem conflitos e o número de usuários que não têm informações de disponibilidade em uma distribuição listam para um sugerida a hora da reunião.
ms.openlocfilehash: 382b4d866c95de98bd444cd6226d71813889d4f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823757"
---
# <a name="groupattendeeconflictdata"></a>GroupAttendeeConflictData

O elemento **GroupAttendeeConflictData** contém informações de conflito agregadas sobre o número de usuários que estão disponíveis, o número de usuários que possuem conflitos e o número de usuários que não têm informações de disponibilidade em uma lista de distribuição para um horário de reunião sugeridas. 
  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [SuggestionsResponse](suggestionsresponse.md)
- [SuggestionDayResultArray](suggestiondayresultarray.md)
- [SuggestionDayResult](suggestiondayresult.md)
- [SuggestionArray](suggestionarray.md)
- [Sugestão](suggestion.md)
- [AttendeeConflictDataArray](attendeeconflictdataarray.md)
- [GroupAttendeeConflictData](groupattendeeconflictdata.md)
  
```xml
<GroupAttendeeConflictData>
   <NumberOfMembers>...</NumberOfMembers>
   <NumberOfMembersAvailable>...</NumberOfMembersAvailable>
   <NumberOfMembersWithConflict>...</NumberOfMembersWithConflict>
   <NumberOfMembersWithNoData>...</NumberOfMembersWithNoData>
</GroupAttendeeConflictData>
```

**GroupAttendeeConflictData**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[NumberOfMembers](numberofmembers.md) <br/> |Representa o número de usuários, recursos e salas em uma lista de distribuição.  <br/> |
|[NumberOfMembersAvailable](numberofmembersavailable.md) <br/> |Representa o número de membros da lista de distribuição que estão disponíveis para um horário de reunião sugeridas. Esse elemento representa membros para o qual o status é **livre**.  <br/> |
|[NumberOfMembersWithConflict](numberofmemberswithconflict.md) <br/> |Representa o número de membros da lista de distribuição que têm um conflito com um tempo de reunião sugeridas. Esse elemento representa membros que possuem um status **ocupado**, **ausência temporária**ou **provisória** .  <br/> |
|[NumberOfMembersWithNoData](numberofmemberswithnodata.md) <br/> |Representa o número de membros de grupo que não têm dados publicados livre/ocupado para comparar com um tempo de reunião sugeridas. Este elemento representa membros de uma lista de distribuição é muito grande ou membros que possuem o status de **Nenhum dado** .  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AttendeeConflictDataArray](attendeeconflictdataarray.md) <br/> |Contém uma matriz de dados de conflito para participantes consultados identificados na [operação GetUserAvailability](getuseravailability-operation.md).  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a>Coment�rios

O elemento **GroupAttendeeConflictData** está presente na resposta quando um participante do [GetUserAvailabilityRequest](getuseravailabilityrequest.md) é resolvido para uma lista de distribuição. O elemento **GroupAttendeeConflictData** identifica três estados para membros de uma lista de distribuição: disponível, em conflito, ou nenhum dado. Expansão de lista de distribuição dará suporte a até 100 membros. Portanto, o elemento [NumberOfMembers](numberofmembers.md) pode conter um máximo de 100 membros. Expansão de lista de distribuição é recursiva. Se uma lista de distribuição contiver uma lista de distribuição de filhos que expande a associação do pai total a mais de 100 membros, na lista de distribuição de filhos não podem ser expandida e contará como uma única entrada da contagem do elemento [NumberOfMembersWithNoData](numberofmemberswithnodata.md) . Se uma lista de distribuição filho pode ser expandida e a associação de total pai não expande a mais de 100 membros, sua associação é expandida e as contagens do membro são adicionadas aos elementos filho do elemento **GroupAttendeeConflictData** . 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [Obtenção de disponibilidade do usuário](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

