---
title: DeleteItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItemField
api_type:
- schema
ms.assetid: 3893be6a-49a7-49f6-bf53-c7f819ec3f87
description: O elemento DeleteItemField representa uma operação para excluir uma determinada propriedade de um item durante uma chamada de UpdateItem.
ms.openlocfilehash: 2388bd10379211a31890b7c4f27920431ce444c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751754"
---
# <a name="deleteitemfield"></a>DeleteItemField

O elemento **DeleteItemField** representa uma operação para excluir uma determinada propriedade de um item durante uma chamada de UpdateItem. 
 
- [UpdateItem](updateitem.md)  
- [ItemChanges](itemchanges.md) 
- [ItemChange](itemchange.md) 
- [Atualizações (Item)](updates-item.md) 
- [DeleteItemField](deleteitemfield.md)
  
```xml
<DeleteItemField>
   <FieldURI/>
</DeleteItemField>
```

 **DeleteItemFieldType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifica as propriedades frequentemente referenciadas pelo URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifica a membros individuais de uma propriedade de dicionário.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica as propriedades estendidas de MAPI.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Atualizações (Item)](updates-item.md) <br/> |Contém um conjunto de elementos que definem append, definir e excluir as alterações nas propriedades do item.  <br/><br/>Este é a expressão XPath para esse elemento:<br/>`/UpdateItem/ItemChanges/ItemChange[i]/Updates` <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação UpdateItem](updateitem-operation.md)

