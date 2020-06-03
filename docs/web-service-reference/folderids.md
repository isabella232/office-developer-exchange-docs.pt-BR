---
title: FolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderIds
api_type:
- schema
ms.assetid: 3ff9d15a-7220-4785-ae6b-583a7eb82005
description: O elemento FolderIds contém uma matriz de identificadores de pasta que são usados para identificar as pastas a serem copiadas, movidas, obtidas, excluídas ou monitoradas para notificações de eventos.
ms.openlocfilehash: ff0476f72c7da088bd2b39f58ab560dcc82197e4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530990"
---
# <a name="folderids"></a>FolderIds

O elemento **FolderIds** contém uma matriz de identificadores de pasta que são usados para identificar as pastas a serem copiadas, movidas, obtidas, excluídas ou monitoradas para notificações de eventos. 
  
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
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifica as pastas do Microsoft Exchange Server que podem ser referenciadas por nome.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetFolder](getfolder.md) <br/> |Define uma solicitação para obter uma pasta do repositório do Exchange.  <br/> A seguir está a expressão XPath para este elemento:`/GetFolder` <br/> |
|[DeleteFolder](deletefolder.md) <br/> |Define uma solicitação para excluir pastas do repositório do Exchange.  <br/> A seguir está a expressão XPath para este elemento:`/DeleteFolder` <br/> |
|[EmptyFolder](emptyfolder.md) <br/> |Define uma solicitação para excluir pastas do repositório do Exchange.  <br/> A seguir está a expressão XPath para este elemento:`/EmptyFolder` <br/> |
|[MoveFolder](movefolder.md) <br/> |Define uma solicitação para mover uma pasta no repositório do Exchange.  <br/> A seguir está a expressão XPath para este elemento:`/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Define uma solicitação para copiar uma pasta no repositório do Exchange.  <br/> A seguir está a expressão XPath para este elemento:`/CopyFolder` <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Representa uma assinatura para uma assinatura de notificação de eventos baseada em push.  <br/> |
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |Representa uma assinatura para uma assinatura de notificação de eventos baseada em pull.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages e https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens; Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Messages. xsd; Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetFolder](getfolder-operation.md)
  
[Operação DeleteFolder](deletefolder-operation.md)
  
[Operação MoveFolder](movefolder-operation.md)
  
[Operação CopyFolder](copyfolder-operation.md)
  
[Operação Subscribe](subscribe-operation.md)

