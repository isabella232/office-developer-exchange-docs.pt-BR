---
title: Excluir (ItemSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- schema
ms.assetid: 4f372d57-2e39-46af-9d83-6c8c55108587
description: O elemento de excluir identifica um único item a ser excluído no repositório de cliente local.
ms.openlocfilehash: 18b7ae2f97db2de64896680c3aa76f2590c03177
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751733"
---
# <a name="delete-itemsync"></a>Excluir (ItemSync)

O elemento de **Excluir** identifica um único item a ser excluído no repositório de cliente local. 
  
- [SyncFolderItemsResponse](syncfolderitemsresponse.md)  
- [ResponseMessages](responsemessages.md) 
- [SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)  
- [Alterações (itens)](changes-items.md)  
- [Excluir (ItemSync)](delete-itemsync.md)
  
```xml
<Delete>
   <ItemId/>
</Delete>
```

**SyncFolderItemsDeleteType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |Contém o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Alterações (itens)](changes-items.md) <br/> |Contém uma matriz de sequência de tipos de alteração que representam o tipo das diferenças entre os itens no cliente e os itens no servidor Exchange.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação SyncFolderItems](syncfolderitems-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

