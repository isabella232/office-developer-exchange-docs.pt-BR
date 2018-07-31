---
title: ExtendedProperty
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExtendedProperty
api_type:
- schema
ms.assetid: f9701409-b620-4afe-b9ee-4c1e95507af7
description: O elemento ExtendedProperty identifica as propriedades estendidas de MAPI em pastas e itens.
ms.openlocfilehash: 9a6c44e953cab4900e4b75eb42bdf4d8633e58f9
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353725"
---
# <a name="extendedproperty"></a>ExtendedProperty

O elemento **ExtendedProperty** identifica as propriedades estendidas de MAPI em pastas e itens. 
  
```xml
<ExtendedProperty>
   <ExtendedFieldURI/>
   <Values/>
</ExtendedProperty>
```

```xml
<ExtendedProperty>
   <ExtendedFieldURI/>
   <Value/>
</ExtendedProperty>
```

**ExtendedPropertyType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica uma propriedade MAPI estendida para obter, definir ou criar.  <br/> |
|[Values](values.md) <br/> |Contém uma coleção de valores de uma propriedade MAPI estendida multivalorado.  <br/> |
|[Valor](value.md) <br/> |Contém o valor da propriedade estendida de MAPI valor único.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato do Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[1.1](item.md) <br/> |Representa um item no armazenamento do Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa o cancelamento da reunião no armazenamento do Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no armazenamento do Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no armazenamento do Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no armazenamento do Exchange.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem de email do Exchange.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Remove um item de armazenamento do Exchange.  <br/> |
|[Task](task.md) <br/> |Representa uma tarefa no armazenamento do Exchange.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Representa uma pasta que contém principalmente itens de calendário.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Representa uma pasta de contatos em uma caixa de correio.  <br/> |
|[Folder](folder.md) <br/> |Representa uma pasta para criar, obter, encontre, sincronizar ou atualizar.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Representa uma pasta de pesquisa que está contida em uma caixa de correio.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Representa uma pasta de tarefas que está contida em uma caixa de correio.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

