---
title: SyncFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderId
api_type:
- schema
ms.assetid: 3645fa03-236d-4e5f-b8b9-5d98f7f35fa2
description: O elemento SyncFolderId representa a pasta que contém os itens a serem sincronizados.
ms.openlocfilehash: c90a20095ca4706f0c6edae3e98eaadd6024d817
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354397"
---
# <a name="syncfolderid"></a>SyncFolderId

O elemento **SyncFolderId** representa a pasta que contém os itens a serem sincronizados. 
  
```xml
<SyncFolderId>
   <FolderId/>
</SyncFolderId>
```

```xml
<SyncFolderId>
   <DistinguishedFolderId/> 
</SyncFolderId>
```

**TargetFolderIdType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contém o identificador e alterar a chave de uma pasta.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifica as pastas de MicrosoftExchange Server 2007 que podem ser referidas por nome.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SyncFolderHierarchy](syncfolderhierarchy.md) <br/> |Define uma solicitação para sincronizar uma hierarquia de pastas em um repositório do Exchange.  <br/> |
|[SyncFolderItems](syncfolderitems.md) <br/> |Define uma solicitação para sincronizar os itens em uma pasta de repositório do Exchange.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação SyncFolderItems](syncfolderitems-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

