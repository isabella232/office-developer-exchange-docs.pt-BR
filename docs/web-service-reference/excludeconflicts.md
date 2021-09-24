---
title: ExcludeConflicts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExcludeConflicts
api_type:
- schema
ms.assetid: ec33ef23-8537-41eb-8d89-7eb906a1fad7
description: O elemento ExcludeConflicts especifica se é preciso retornar os horários sugeridos para os horários de calendário que conflitam entre os participantes.
ms.openlocfilehash: 6182ff8faed62cefc39015d3242bf7e669660b4a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539905"
---
# <a name="excludeconflicts"></a>ExcludeConflicts

O **elemento ExcludeConflicts** especifica se é preciso retornar os horários sugeridos para os horários de calendário que conflitam entre os participantes. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[MailboxDataArray](mailboxdataarray.md)
  
[MailboxData](mailboxdata.md)
  
[ExcludeConflicts](excludeconflicts.md)
  
```xml
<ExcludeConflicts>true or false</ExcludeConflicts>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MailboxData](mailboxdata.md) <br/> |Representa um usuário de caixa de correio individual e opções para o tipo de dados a serem retornados sobre o usuário da caixa de correio.  <br/> Veja a seguir o XPath para este elemento:  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. Os valores possíveis são um Boolean **true** ou **false**.
  
## <a name="remarks"></a>Comentários

Este elemento é obrigatório.
  
> [!NOTE]
> O esquema que descreve esse elemento está localizado no diretório /EWS/do computador que está executando o MicrosoftExchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserAvailability](getuseravailability-operation.md)
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)


[Obter Disponibilidade do Usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

