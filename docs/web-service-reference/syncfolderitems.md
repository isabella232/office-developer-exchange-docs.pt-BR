---
title: SyncFolderItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 463ed78c-bf82-4cd8-971a-d18425e9e7be
description: O elemento SyncFolderItems define uma solicitação para sincronizar itens em uma pasta Exchange store.
ms.openlocfilehash: a3e5aa83335a6bc29b832021e227e6adad4092bf
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513280"
---
# <a name="syncfolderitems"></a>SyncFolderItems

O **elemento SyncFolderItems** define uma solicitação para sincronizar itens em uma Exchange de armazenamento. 
  
```xml
<SyncFolderItems>
   <ItemShape/>
   <SyncFolderId/>
   <SyncState/>
   <Ignore/>
   <MaxChangesReturned/>   <SyncScope/>
</SyncFolderItems>
```

 **SyncFolderItemsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |Identifica as propriedades do item e o conteúdo a ser incluído em uma resposta SyncFolderItems. Este elemento é obrigatório.  <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Representa a pasta que contém os itens a sincronizar. Este elemento é obrigatório.  <br/> |
|[SyncState](syncstate-ex15websvcsotherref.md) <br/> |Contém uma forma codificada com base64 dos dados de sincronização que são atualizados após cada solicitação bem-sucedida. Isso é usado para identificar o estado de sincronização. Esse elemento é opcional.  <br/> |
|[Ignore](ignore.md) <br/> |Identifica itens a ignorar durante a sincronização. Esse elemento é opcional.  <br/> |
|[MaxChangesReturned](maxchangesreturned.md) <br/> |Descreve o número máximo de alterações que podem ser retornadas em uma resposta de sincronização. Este elemento é obrigatório.  <br/> |
|[SyncScope](syncscope.md) <br/> |Especifica se apenas itens ou itens e informações associadas a pastas são retornadas em uma resposta de sincronização. Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação SyncFolderItems](syncfolderitems-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

