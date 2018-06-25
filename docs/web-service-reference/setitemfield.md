---
title: SetItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetItemField
api_type:
- schema
ms.assetid: 85284fcb-bd1e-4fda-9dab-cb4cd637cd5b
description: O elemento SetItemField representa uma atualização para uma única propriedade de um item em uma operação UpdateItem.
ms.openlocfilehash: 012e6ae21af653b4bf12588e5a97334a62884059
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825439"
---
# <a name="setitemfield"></a>SetItemField

O elemento **SetItemField** representa uma atualização para uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).
  
```xml
<SetItemField>
   <FieldURI/>
   <Item/>
</SetItemField>
```

 **SetItemFieldType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifica as propriedades frequentemente referenciadas pelo URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifica a membros individuais de um dicionário.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica as propriedades estendidas de MAPI para definir.  <br/> |
|[1.1](item.md) <br/> |Representa um item no armazenamento do Exchange.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem de email do Exchange para atualizar.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange para atualizar.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato do Exchange para atualizar.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição a ser atualizado.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma mensagem de reunião a atualização.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião para atualizar.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião para atualizar.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa o cancelamento da reunião para atualizar.  <br/> |
|[Task](task.md) <br/> |Representa uma tarefa a ser atualizado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Atualizações (Item)](updates-item.md) <br/> |Contém um conjunto de elementos que definem append, definir e excluir as alterações nas propriedades do item.  <br/> |
   
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



[Operação UpdateItem](updateitem-operation.md)

