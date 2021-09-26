---
title: SyncState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SyncState
api_type:
- schema
ms.assetid: e5ebaae3-0f07-481d-ac67-d9687a3c7ac3
description: O elemento SyncState contém uma forma codificada com base64 dos dados de sincronização que são atualizados após cada solicitação bem-sucedida. Isso é usado para identificar o estado de sincronização.
ms.openlocfilehash: 72a0e347b5732cbe397956f8cc50b3266fba9156
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543902"
---
# <a name="syncstate"></a>SyncState

O **elemento SyncState** contém uma forma codificada com base64 dos dados de sincronização que são atualizados após cada solicitação bem-sucedida. Isso é usado para identificar o estado de sincronização. 
  
```xml
<SyncState/>
```

 **String**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SyncFolderHierarchy](syncfolderhierarchy.md) <br/> |Define uma solicitação para sincronizar uma hierarquia de pastas em um cliente.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação SyncFolderHierarchy.  <br/> |
|[SyncFolderItems](syncfolderitems.md) <br/> |Define uma solicitação para sincronizar itens em uma pasta Exchange store.  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação SyncFolderItems.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário quando esse elemento é usado.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação SyncFolderItems](syncfolderitems-operation.md)
  
[Operação SyncFolderHierarchy](syncfolderhierarchy-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

