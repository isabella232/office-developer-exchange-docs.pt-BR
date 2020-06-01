---
title: SyncFolderItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 463ed78c-bf82-4cd8-971a-d18425e9e7be
description: O elemento SyncFolderItems define uma solicitação para sincronizar itens em uma pasta do repositório do Exchange.
ms.openlocfilehash: 0fa5b1544d5627d1423287369e72f97662c28d12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465146"
---
# <a name="syncfolderitems"></a>SyncFolderItems

O elemento **SyncFolderItems** define uma solicitação para sincronizar itens em uma pasta do repositório do Exchange. 
  
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
|[Shape](itemshape.md) <br/> |Identifica as propriedades e o conteúdo do item que serão incluídos em uma resposta SyncFolderItems. Este elemento é obrigatório.  <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Representa a pasta que contém os itens a serem sincronizados. Este elemento é obrigatório.  <br/> |
|[SyncState](syncstate-ex15websvcsotherref.md) <br/> |Contém uma forma codificada em base64 dos dados de sincronização que são atualizados após cada solicitação bem-sucedida. Isso é usado para identificar o estado de sincronização. Este elemento é opcional.  <br/> |
|[Ignore](ignore.md) <br/> |Identifica os itens a serem ignorados durante a sincronização. Este elemento é opcional.  <br/> |
|[MaxChangesReturned](maxchangesreturned.md) <br/> |Descreve o número máximo de alterações que podem ser retornadas em uma resposta de sincronização. Este elemento é obrigatório.  <br/> |
|[SyncScope](syncscope.md) <br/> |Especifica se apenas itens ou itens e informações associadas à pasta são retornados em uma resposta de sincronização. Este elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação SyncFolderItems](syncfolderitems-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

