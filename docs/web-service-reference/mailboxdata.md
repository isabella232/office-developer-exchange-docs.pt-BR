---
title: MailboxData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailboxData
api_type:
- schema
ms.assetid: e9e3f50c-5a7b-49c7-a9ea-117959c08352
description: O elemento MailboxData representa um usuário de caixa de correio individual e opções para o tipo de dados a serem retornados sobre o usuário da caixa de correio.
ms.openlocfilehash: 62c8c816fc0b0e0c6831d468d90e7303fb72d9be
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546130"
---
# <a name="mailboxdata"></a>MailboxData

O **elemento MailboxData** representa um usuário de caixa de correio individual e opções para o tipo de dados a serem retornados sobre o usuário da caixa de correio. 
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
- [MailboxDataArray](mailboxdataarray.md)
  
- [MailboxData](mailboxdata.md)
  
```xml
<MailboxData>
   <Email>...</Email>
   <AttendeeType>...</AttendeeType>
   <ExcludeConflicts>...</ExcludeConflicts>
<MailboxData>
```

**MailboxData**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Email (EmailAddressType)](email-emailaddresstype.md) <br/> |Representa o usuário da caixa de correio para uma consulta GetUserAvailability.  <br/> |
|[AttendeeType](attendeetype.md) <br/> |Representa o tipo de participante identificado no [elemento Email (EmailAddressType).](email-emailaddresstype.md) Isso é usado em solicitações para sugestões de reunião.  <br/> |
|[ExcludeConflicts](excludeconflicts.md) <br/> |Especifica se é preciso retornar os horários sugeridos para os horários de calendário que conflitam entre os participantes.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MailboxDataArray](mailboxdataarray.md) <br/> |Contém uma lista de caixas de correio para consultar informações de disponibilidade.  <br/> Veja a seguir o XPath para este elemento:  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]` <br/> |
   
## <a name="remarks"></a>Comentários

Um aplicativo cliente pode definir um para muitos elementos **MailboxData.** 
  
> [!NOTE]
> O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada. 
  
## <a name="example"></a>Exemplo

```xml
<MailboxDataArray>
  <MailboxData xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
    <Email>
      <Name></Name>
      <Address>someone@ExServer.example.com</Address>
      <RoutingType>SMTP</RoutingType>
    </Email>
    <AttendeeType>Organizer</AttendeeType>
    <ExcludeConflicts>false</ExcludeConflicts>
  </MailboxData>
</MailboxDataArray>
```

## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [Obter Disponibilidade do Usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

