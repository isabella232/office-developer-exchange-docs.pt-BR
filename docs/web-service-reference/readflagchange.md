---
title: ReadFlagChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ReadFlagChange
api_type:
- schema
ms.assetid: 527bfe90-63d0-4b2f-97f7-7875b3a516b2
description: O elemento ReadFlagChange é retornado nas respostas da operação SyncFolderItems quando um item foi lido. Essa propriedade é somente leitura.
ms.openlocfilehash: 8a03f32a54b2e9dd7e84bf77a01092f6bb3cbf19
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542908"
---
# <a name="readflagchange"></a>ReadFlagChange

O **elemento ReadFlagChange** é retornado nas respostas da operação [SyncFolderItems](syncfolderitems-operation.md) quando um item foi lido. Essa propriedade é somente leitura. 
  
```xml
<ReadFlagChange>
   <ItemId/>
   <IsRead/>
</ReadFlagChange>
```

 **SyncFolderItemsReadFlagType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |Identifica o item para o qual o sinalizador de leitura foi alterado.  <br/> |
|[IsRead](isread.md) <br/> |Indica se o sinalizador de leitura foi definido como **true**.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Changes (Items)](changes-items.md) <br/> |Contém uma matriz de sequência de tipos de alteração que representam os tipos de diferenças entre os itens no cliente e os itens no Exchange servidor.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2010 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

