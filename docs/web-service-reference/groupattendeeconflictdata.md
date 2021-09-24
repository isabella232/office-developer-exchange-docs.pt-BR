---
title: GroupAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GroupAttendeeConflictData
api_type:
- schema
ms.assetid: fd8bf19a-298b-4135-93e8-ead3db7e1142
description: O elemento GroupAttendeeConflictData contém informações de conflito agregadas sobre o número de usuários disponíveis, o número de usuários que têm conflitos e o número de usuários que não têm informações de disponibilidade em uma lista de distribuição para um horário de reunião sugerido.
ms.openlocfilehash: 19ac366da5ad48cbc6c9e2aaa710a8c5f00e1151
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519552"
---
# <a name="groupattendeeconflictdata"></a>GroupAttendeeConflictData

O **elemento GroupAttendeeConflictData** contém informações de conflito agregadas sobre o número de usuários disponíveis, o número de usuários que têm conflitos e o número de usuários que não têm informações de disponibilidade em uma lista de distribuição para um horário de reunião sugerido. 
  
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

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[NumberOfMembers](numberofmembers.md) <br/> |Representa o número de usuários, recursos e salas em uma lista de distribuição.  <br/> |
|[NumberOfMembersAvailable](numberofmembersavailable.md) <br/> |Representa o número de membros da lista de distribuição que estão disponíveis para um horário de reunião sugerido. Este elemento representa membros para os quais o status é **Free**.  <br/> |
|[NumberOfMembersWithConflict](numberofmemberswithconflict.md) <br/> |Representa o número de membros da lista de distribuição que têm um conflito com um horário de reunião sugerido. Esse elemento representa membros que têm um status **Ocupado,** **OOF** ou **Tentativo.**  <br/> |
|[NumberOfMembersWithNoData](numberofmemberswithnodata.md) <br/> |Representa o número de membros do grupo que não publicaram dados de ocupado/livre para comparar com um horário de reunião sugerido. Esse elemento representa membros de uma lista de distribuição muito grande ou membros que não **têm status de** Dados.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AttendeeConflictDataArray](attendeeconflictdataarray.md) <br/> |Contém uma matriz de dados de conflito para participantes consultados identificados na [operação GetUserAvailability](getuseravailability-operation.md).  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a>Comentários

O **elemento GroupAttendeeConflictData** está presente na resposta quando um participante no [GetUserAvailabilityRequest](getuseravailabilityrequest.md) é resolvido para uma lista de distribuição. O **elemento GroupAttendeeConflictData** identifica três estados para membros de uma lista de distribuição: disponíveis, conflitantes ou sem dados. A expansão da lista de distribuição terá suporte para até 100 membros. Portanto, o [elemento NumberOfMembers](numberofmembers.md) pode conter no máximo 100 membros. A expansão da lista de distribuição é recursiva. Se uma lista de distribuição contiver uma lista de distribuição filho que expanda a associação pai total para mais de 100 membros, a lista de distribuição filho não será expandida e contará como uma única entrada da contagem de elementos [NumberOfMembersWithNoData.](numberofmemberswithnodata.md) Se uma lista de distribuição filho puder ser expandida e a associação pai total não se expandir para mais de 100 membros, sua associação será expandida e as contagens de membros serão adicionadas aos elementos filho do **elemento GroupAttendeeConflictData.** 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [Obter Disponibilidade do Usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

