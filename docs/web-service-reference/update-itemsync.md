---
title: Update (ItemSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Update
api_type:
- schema
ms.assetid: 4e204446-1c80-44f9-b93b-77ce630a01a5
description: O elemento Update identifica um único item a ser atualizado no armazenamento de cliente local.
ms.openlocfilehash: 936226c671916b974eed9dea9ad2ea39bde482a9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541816"
---
# <a name="update-itemsync"></a>Update (ItemSync)

O **elemento Update** identifica um único item a ser atualizado no armazenamento de cliente local. 
  
- [SyncFolderItemsResponse](syncfolderitemsresponse.md) 
- [ResponseMessages](responsemessages.md)  
- [SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)  
- [Changes (Items)](changes-items.md)  
- [Update (ItemSync)](update-itemsync.md)
  
```xml
<Update>
   <Item/>
</Update>
```

```xml
<Update>
   <MeetingRequest/>
</Update>
```

```xml
<Update>
   <MeetingCancellation/>
</Update>
```

```xml
<Update>
   <Task/>
</Update>
```

```xml
<Update>
   <CalendarItem/>
</Update>
```

```xml
<Update>
   <MeetingResponse/>
</Update>
```

```xml
<Update>
   <Message/>
</Update>
```

```xml
<Update>
   <DistributionList/>
</Update>
```

```xml
<Update>
   <MeetingMessage/>
</Update>
```

```xml
<Update>
   <Contact/> 
</Update>
```

**SyncFolderItemsCreateOrUpdateType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Item](item.md) <br/> |Representa um item Exchange genérico a ser atualizado.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma Exchange de email a ser atualizada.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um Exchange de calendário a ser atualizado.  <br/> |
|[Contato](contact.md) <br/> |Representa um Exchange de contato a ser atualizado.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição a ser atualizada.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma mensagem de reunião a ser atualizada.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião a ser atualizada.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião para atualização.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião a ser atualizado.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa a ser atualizada.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Changes (Items)](changes-items.md) <br/> |Contém uma matriz de sequência de tipos de alteração que representam o tipo de diferenças entre os itens no cliente e os itens no servidor Exchange.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação SyncFolderItems](syncfolderitems-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

