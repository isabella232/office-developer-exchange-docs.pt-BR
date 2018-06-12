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
description: O elemento de SyncFolderItems define uma solicitação para sincronizar os itens em uma pasta de repositório do Exchange.
ms.openlocfilehash: 368e19babfccaeab40380103495c63d30647905c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837686"
---
# <a name="syncfolderitems"></a>SyncFolderItems

O elemento de **SyncFolderItems** define uma solicitação para sincronizar os itens em uma pasta de repositório do Exchange. 
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |Identifica as propriedades do item e o conteúdo a ser incluído em uma resposta SyncFolderItems. Este elemento é obrigatório.  <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Representa a pasta que contém os itens a serem sincronizados. Este elemento é obrigatório.  <br/> |
|[Estado de sincronização](syncstate-ex15websvcsotherref.md) <br/> |Contém um formulário codificado na base64 dos dados de sincronização que são atualizados após cada solicitação bem-sucedida. Isso é usado para identificar o estado de sincronização. Esse elemento é opcional.  <br/> |
|[Ignore](ignore.md) <br/> |Identifica os itens a serem ignorados durante a sincronização. Esse elemento é opcional.  <br/> |
|[MaxChangesReturned](maxchangesreturned.md) <br/> |Descreve o número máximo de alterações que pode ser retornado em uma resposta de sincronização. Este elemento é obrigatório.  <br/> |
|[SyncScope](syncscope.md) <br/> |Especifica se apenas itens ou itens e informações de pasta associada são retornados em uma resposta de sincronização. Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação SyncFolderItems](syncfolderitems-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

