---
title: AllowNewTimeProposal
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AllowNewTimeProposal
api_type:
- schema
ms.assetid: afdb4ec9-2daf-48a1-a0bb-a7f647f212f2
description: O elemento AllowNewTimeProposal indica se um novo horário de reunião pode ser proposto para uma reunião por um participante.
ms.openlocfilehash: 1acb95189e1949204a25f97a82770b88590df776
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543727"
---
# <a name="allownewtimeproposal"></a>AllowNewTimeProposal

O **elemento AllowNewTimeProposal** indica se um novo horário de reunião pode ser proposto para uma reunião por um participante. 
  
```xml
<AllowNewTimeProposal/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhuma
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma reunião no Exchange store.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um Exchange de calendário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa um valor Boolean é necessário. Um valor **verdadeiro** indica que uma nova proposta para o horário da reunião pode ser criada; um valor **false** indica que novas propostas de tempo não são permitidas. O organizador define esse valor na solicitação de reunião. 
  
## <a name="remarks"></a>Comentários

A propriedade AllowNewTimeProposal pode ser lida para o item de calendário do organizador. Ele é somente leitura para solicitações de reunião e itens de calendário dos participantes.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
> [!NOTE]
> Exchange Os Serviços Web não suportam novas mensagens de proposta de tempo. Para obter propriedades relacionadas a novas mensagens de proposta de tempo, use propriedades estendidas. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

