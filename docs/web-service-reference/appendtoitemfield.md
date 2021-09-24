---
title: AppendToItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AppendToItemField
api_type:
- schema
ms.assetid: 66dbcb4a-ae6d-4648-8610-67187bdb105c
description: O elemento AppendToItemField identifica dados a ser anexados a uma única propriedade de um item durante uma operação UpdateItem.
ms.openlocfilehash: 8e94ca9174d11f1f6e4a0dd2fcfabeb30a64a40d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540325"
---
# <a name="appendtoitemfield"></a>AppendToItemField

O **elemento AppendToItemField** identifica dados a ser anexados a uma única propriedade de um item durante uma [operação UpdateItem.](updateitem-operation.md)
  
- [UpdateItem](updateitem.md)
  
- [ItemChanges](itemchanges.md)
  
- [ItemChange](itemchange.md)
  
- [Updates (Item)](updates-item.md)
  
- [AppendToItemField](appendtoitemfield.md)
  
```xml
<AppendToItemField>
   <FieldURI/>
   <Item/>
</AppendToItemField>
```

 **AppendToItemFieldType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifica propriedades referenciadas com frequência por URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifica membros individuais de um dicionário.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica propriedades MAPI estendidas a ser anexadas.  <br/> |
|[Item](item.md) <br/> |Representa um item no Exchange store.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma Exchange de email.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um Exchange de calendário.  <br/> |
|[Contato](contact.md) <br/> |Representa um Exchange de contato.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no Exchange store.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no Exchange store.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no Exchange store.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no Exchange store.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no Exchange store.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Updates (Item)](updates-item.md) <br/> |Contém uma matriz que define anexar, definir e excluir alterações nas propriedades do item.  <br/> Veja a seguir a expressão XPath para este elemento:  `/UpdateItem/ItemChanges/ItemChange[i]/Updates` <br/> |
   
## <a name="remarks"></a>Comentários

Somente determinadas propriedades suportam operações de anexação. Uma tentativa de anexar a uma propriedade que não oferece suporte à anexação resultará em um erro.
  
Para operações de atualização, apenas uma propriedade pode ser modificada em uma única solicitação. Essa propriedade única deve ser referenciada no [elemento Path.](path.md) O **elemento Item** nas classes derivadas só pode conter uma única propriedade que está em acordo com o único elemento **Path.** 
  
> [!NOTE]
> O [elemento Path](path.md) é abstrato. Ele deve ser substituído pelo [elemento FieldURI,](fielduri.md) [IndexedFieldURI](indexedfielduri.md)ou [ExtendedFieldURI.](extendedfielduri.md) 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação UpdateItem](updateitem-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

