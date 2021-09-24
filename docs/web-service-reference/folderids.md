---
title: FolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FolderIds
api_type:
- schema
ms.assetid: 3ff9d15a-7220-4785-ae6b-583a7eb82005
description: O elemento FolderIds contém uma matriz de identificadores de pasta que são usados para identificar pastas para copiar, mover, obter, excluir ou monitorar notificações de eventos.
ms.openlocfilehash: 7c0cf46d5fdaf35ec72cf3b5750b51edc5a8bfe0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518362"
---
# <a name="folderids"></a>FolderIds

O **elemento FolderIds** contém uma matriz de identificadores de pasta que são usados para identificar pastas para copiar, mover, obter, excluir ou monitorar notificações de eventos. 
  
```xml
<FolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</FolderIds>
```

 **NonEmptyArrayOfBaseFolderIdsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contém o identificador e a chave de alteração de uma pasta.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifica Microsoft Exchange Server pastas que podem ser referenciadas pelo nome.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetFolder](getfolder.md) <br/> |Define uma solicitação para obter uma pasta do Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  `/GetFolder` <br/> |
|[DeleteFolder](deletefolder.md) <br/> |Define uma solicitação para excluir pastas do Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  `/DeleteFolder` <br/> |
|[EmptyFolder](emptyfolder.md) <br/> |Define uma solicitação para excluir pastas do Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  `/EmptyFolder` <br/> |
|[MoveFolder](movefolder.md) <br/> |Define uma solicitação para mover uma pasta no Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  `/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Define uma solicitação para copiar uma pasta no Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  `/CopyFolder` <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Representa uma assinatura de uma assinatura de notificação de evento baseada em push.  <br/> |
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |Representa uma assinatura de uma assinatura de notificação de evento baseada em pull.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages e https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens; Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Messages.xsd; Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetFolder](getfolder-operation.md)
  
[Operação DeleteFolder](deletefolder-operation.md)
  
[Operação MoveFolder](movefolder-operation.md)
  
[Operação CopyFolder](copyfolder-operation.md)
  
[Operação de assinatura](subscribe-operation.md)

