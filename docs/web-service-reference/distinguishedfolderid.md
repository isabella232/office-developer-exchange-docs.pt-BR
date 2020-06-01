---
title: DistinguishedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistinguishedFolderId
api_type:
- schema
ms.assetid: 50018162-2941-4227-8a5b-d6b4686bb32f
description: O elemento DistinguishedFolderId identifica pastas que podem ser referenciadas por nome. Se você não usar esse elemento, você deve usar o elemento FolderId para identificar uma pasta.
ms.openlocfilehash: be883cbca00910b24e4c45ba047803e5a5024566
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462693"
---
# <a name="distinguishedfolderid"></a>DistinguishedFolderId

O elemento **DistinguishedFolderId** identifica pastas que podem ser referenciadas por nome. Se você não usar esse elemento, você deve usar o elemento [FolderId](folderid.md) para identificar uma pasta. 
  
```XML
<DistinguishedFolderId Id="" ChangeKey="">
   <Mailbox/>
</DistinguishedFolderId>
```

 **DistinguishedFolderIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Id** <br/> |Contém uma cadeia de caracteres que identifica uma pasta padrão. Esse atributo é necessário.  <br/> |
|**ChangeKey** <br/> |Contém uma cadeia de caracteres que identifica uma versão de uma pasta identificada pelo atributo **ID** . Esse atributo é opcional. Use este atributo para certificar-se de que a versão correta de uma pasta é usada.  <br/> |
   
#### <a name="id-attribute-values"></a>Valores de atributo de ID

|**Valor**|**Descrição**|
|:-----|:-----|
|calendário  <br/> |Representa a pasta calendário.  <br/> |
|contacts  <br/> |Representa a pasta contatos.  <br/> |
|deleteditems  <br/> |Representa a pasta itens excluídos.  <br/> |
|rascunhos  <br/> |Representa a pasta Rascunhos.  <br/> |
|caixa de entrada  <br/> |Representa a pasta caixa de entrada.  <br/> |
|diário  <br/> |Representa a pasta diário.  <br/> |
|notes  <br/> |Representa a pasta anotações.  <br/> |
|Caixa de saída  <br/> |Representa a pasta de saída.  <br/> |
|sentitems  <br/> |Representa a pasta Itens enviados.  <br/> |
|tarefas  <br/> |Representa a pasta tarefas.  <br/> |
|msgfolderroot  <br/> |Representa a raiz da pasta de mensagens.  <br/> |
|root  <br/> |Representa a raiz da caixa de correio.  <br/> |
|junkemail  <br/> |Representa a pasta lixo eletrônico.  <br/> |
|SearchFolders  <br/> |Representa a pasta pastas de pesquisa.  <br/> |
|postal  <br/> |Representa a pasta caixa postal.  <br/> |
|recoverableitemsroot  <br/> |Representa a pasta raiz do dumpster.  <br/> |
|recoverableitemsdeletions  <br/> |Representa a pasta de exclusões de dumpster.  <br/> |
|recoverableitemsversions  <br/> |Representa a pasta versões de dumpster.  <br/> |
|recoverableitemspurges  <br/> |Representa a pasta de limpezas de dumpster.  <br/> |
|archiveroot  <br/> |Representa a pasta de arquivo-raiz.  <br/> |
|archivemsgfolderroot  <br/> |Representa a pasta de mensagens de arquivo morto raiz.  <br/> |
|archivedeleteditems  <br/> |Representa a pasta itens excluídos por arquivo.  <br/> |
|archiveinbox  <br/> |Representa a pasta caixa de entrada de arquivo morto. As versões do Exchange que começam com o número de compilação 15.00.0913.09 incluem esse valor.  <br/> |
|archiverecoverableitemsroot  <br/> |Representa a pasta raiz de itens recuperáveis.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Representa a pasta arquivos mortos de exclusão de itens recuperáveis.  <br/> |
|archiverecoverableitemsversions  <br/> |Representa a pasta de versões de itens recuperáveis.  <br/> |
|archiverecoverableitemspurges  <br/> |Representa a pasta arquivamento de itens recuperáveis.  <br/> |
|syncissues  <br/> |Representa a pasta problemas de sincronização.  <br/> |
|Conflitos  <br/> |Representa a pasta conflitos.  <br/> |
|localfailures  <br/> |Representa a pasta falhas locais.  <br/> |
|serverfailures  <br/> |Representa a pasta falhas do servidor.  <br/> |
|recipientcache  <br/> |Representa a pasta de cache do destinatário.  <br/> |
|quickcontacts  <br/> |Representa a pasta Contatos rápidos.  <br/> |
|conversationhistory  <br/> |Representa a pasta histórico da conversa.  <br/> |
|adminauditlogs  <br/> |Representa a pasta logs de auditoria de administrador.  <br/> |
|todosearch  <br/> |Representa a pasta de pesquisa todo.  <br/> |
|MyContacts  <br/> |Representa a pasta meus contatos.  <br/> |
|Directory  <br/> |Representa a pasta diretório.  <br/> |
|imcontactlist  <br/> |Representa a pasta de lista de contatos de mensagens instantâneas.  <br/> |
|peopleconnect  <br/> |Representa a pasta pessoas que se conectam.  <br/> |
|favoritos  <br/> |Representa a pasta favoritos.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Caixa de Correio](mailbox.md) <br/> |Identifica um endereço SMTP principal. Endereços de proxy não são permitidos.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |Indica a pasta que é direcionada para ações de conversa que usam pastas.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Indica a pasta de destino para copiar e mover ações de conversa.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> | Identifica a pasta na qual uma nova pasta ou item é criado.  <br/><br/>A seguir estão as expressões XPath para este elemento:<br/><br/>  `/CreateItem/ParentFolderId` <br/><br/>`/CreateFolder/ParentFolderId` <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Identifica as pastas a serem pesquisadas para a [operação FindItem](finditem-operation.md) e a [operação FindFolder](findfolder-operation.md).  <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |Representa a coleção de pastas que será pesquisada para determinar o conteúdo de uma pasta de pesquisa.  <br/> |
|[FolderIds](folderids.md) <br/> |Contém uma matriz de identificadores de pasta que são usados para identificar as pastas a serem copiadas, movidas, obtidas, excluídas ou monitoradas para notificações de eventos.  <br/> |
|[FolderChange](folderchange.md) <br/> |Representa uma coleção de alterações a serem realizadas em uma única pasta.  <br/> <br/>A seguir está a expressão XPath para este elemento:<br/><br/>`/UpdateFolder/FolderChanges/FolderChange`<br/> |
|[ToFolderId](tofolderid.md) <br/> | Representa a pasta de destino para uma pasta ou item copiado ou movido.<br/><br/>A seguir estão as expressões XPath para este elemento:<br/><br/>`/MoveFolder/ToFolderId`<br/><br/>`/CopyFolder/ToFolderId`<br/><br/>`/MoveItem/ToFolderId`<br/><br/>`/CopyItem/ToFolderId` <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> | Identifica a pasta de destino para operações que atualizam, enviam e criam itens no repositório do Exchange.<br/><br/>A seguir estão as expressões XPath para este elemento:<br/><br/>`/CreateItem/SavedItemFolderId`<br/><br/>`/UpdateItem/SavedItemFolderId`<br/><br/>`/SendItem/SavedItemFolderId` <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Representa a pasta que contém os itens a serem sincronizados.  <br/> |
|[Userconfigurationname](userconfigurationname.md) <br/> |Representa o nome de um objeto de configuração do usuário. O nome do objeto de configuração do usuário é o identificador de um objeto de configuração do usuário.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Representa a ID da pasta para a qual os itens de email serão copiados.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Representa a ID da pasta para a qual os itens de email serão movidos.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

Um **DistinguishedFolderId** é resolvido para uma **FolderId**. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Criando pastas (serviços Web do Exchange)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

