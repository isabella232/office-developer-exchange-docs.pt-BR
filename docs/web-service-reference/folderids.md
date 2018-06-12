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
description: O elemento FolderIds contém uma matriz de identificadores de pasta que são usados para identificar pastas para copiar, mover, obter, excluir ou monitorar as notificações de eventos.
ms.openlocfilehash: 911a74ca778ee988c270c16c67620a40656d82d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752333"
---
# <a name="folderids"></a>FolderIds

O elemento **FolderIds** contém uma matriz de identificadores de pasta que são usados para identificar pastas para copiar, mover, obter, excluir ou monitorar as notificações de eventos. 
  
```xml
<FolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</FolderIds>
```

 **NonEmptyArrayOfBaseFolderIdsType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contém o identificador e alterar a chave de uma pasta.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifica as pastas do Microsoft Exchange Server que podem ser referidas por nome.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetFolder](getfolder.md) <br/> |Define uma solicitação para obter uma pasta do Exchange store.  <br/> Este é a expressão XPath para esse elemento:`/GetFolder` <br/> |
|[DeleteFolder](deletefolder.md) <br/> |Define uma solicitação para excluir pastas do Exchange store.  <br/> Este é a expressão XPath para esse elemento:`/DeleteFolder` <br/> |
|[EmptyFolder](emptyfolder.md) <br/> |Define uma solicitação para excluir pastas do Exchange store.  <br/> Este é a expressão XPath para esse elemento:`/EmptyFolder` <br/> |
|[MoveFolder](movefolder.md) <br/> |Define uma solicitação para mover uma pasta no repositório do Exchange.  <br/> Este é a expressão XPath para esse elemento:`/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Define uma solicitação para copiar uma pasta no repositório do Exchange.  <br/> Este é a expressão XPath para esse elemento:`/CopyFolder` <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Representa uma assinatura para uma inscrição de notificação de push com base no evento.  <br/> |
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |Representa uma assinatura para uma inscrição de notificação de evento baseado em extração.  <br/> |
   
## <a name="remarks"></a>Coment�rios

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages e http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens; Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Messages.xsd; Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação GetFolder](getfolder-operation.md)
  
[Operação DeleteFolder](deletefolder-operation.md)
  
[Operação MoveFolder](movefolder-operation.md)
  
[Operação CopyFolder](copyfolder-operation.md)
  
[Inscrever-se a operação](subscribe-operation.md)

