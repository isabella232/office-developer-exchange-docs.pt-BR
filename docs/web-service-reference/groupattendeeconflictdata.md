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
description: O elemento GroupAttendeeConflictData contém informações de conflito de agregação sobre o número de usuários que estão disponíveis, o número de usuários que têm conflitos e o número de usuários que não têm informações de disponibilidade em uma lista de distribuição para um tempo de reunião sugerido.
ms.openlocfilehash: c75a4e6f8fdff7fb2514f448350fee9f1acb9775
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462926"
---
# <a name="groupattendeeconflictdata"></a>GroupAttendeeConflictData

O elemento **GroupAttendeeConflictData** contém informações de conflito de agregação sobre o número de usuários que estão disponíveis, o número de usuários que têm conflitos e o número de usuários que não têm informações de disponibilidade em uma lista de distribuição para um tempo de reunião sugerido. 
  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [SuggestionsResponse](suggestionsresponse.md)
- [SuggestionDayResultArray](suggestiondayresultarray.md)
- [SuggestionDayResult](suggestiondayresult.md)
- [SuggestionArray](suggestionarray.md)
- [La](suggestion.md)
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

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[NumberOfMembers](numberofmembers.md) <br/> |Representa o número de usuários, recursos e salas em uma lista de distribuição.  <br/> |
|[NumberOfMembersAvailable](numberofmembersavailable.md) <br/> |Representa o número de membros da lista de distribuição que estão disponíveis para um tempo de reunião sugerido. Este elemento representa Membros para os quais o status é **livre**.  <br/> |
|[NumberOfMembersWithConflict](numberofmemberswithconflict.md) <br/> |Representa o número de membros da lista de distribuição que têm um conflito com um tempo de reunião sugerido. Este elemento representa os membros que têm um status **ocupado**, **OOF**ou **provisório** .  <br/> |
|[NumberOfMembersWithNoData](numberofmemberswithnodata.md) <br/> |Representa o número de membros do grupo que não publicaram dados de disponibilidade para comparar com um horário de reunião sugerido. Este elemento representa os membros de uma lista de distribuição muito grande ou membros que não têm status de **dados** .  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AttendeeConflictDataArray](attendeeconflictdataarray.md) <br/> |Contém uma matriz de dados de conflito para participantes consultados identificados na [operação GetUserAvailability](getuseravailability-operation.md).  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a>Comentários

O elemento **GroupAttendeeConflictData** está presente na resposta quando um participante do [GetUserAvailabilityRequest](getuseravailabilityrequest.md) é resolvido para uma lista de distribuição. O elemento **GroupAttendeeConflictData** identifica três Estados de membros de uma lista de distribuição: disponível, conflitante ou nenhum dado. A expansão da lista de distribuição suportará até 100 membros. Portanto, o elemento [NumberOfMembers](numberofmembers.md) pode conter um máximo de 100 membros. A expansão da lista de distribuição é recursiva. Se uma lista de distribuição contiver uma lista de distribuição de filhos que expanda a associação pai total para mais de 100 membros, a lista de distribuição secundária não será expandida e será contará como uma única entrada da contagem de elementos [NumberOfMembersWithNoData](numberofmemberswithnodata.md) . Se uma lista de distribuição filha puder ser expandida e a associação pai total não for expandida para mais de 100 membros, sua associação será expandida e as contagens de membro serão adicionadas aos elementos filho do elemento **GroupAttendeeConflictData** . 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [Obtendo disponibilidade do usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

