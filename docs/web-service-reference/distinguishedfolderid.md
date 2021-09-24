---
title: DistinguishedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DistinguishedFolderId
api_type:
- schema
ms.assetid: 50018162-2941-4227-8a5b-d6b4686bb32f
description: O elemento DistinguishedFolderId identifica pastas que podem ser referenciadas pelo nome. Se você não usar esse elemento, deverá usar o elemento FolderId para identificar uma pasta.
ms.openlocfilehash: 309db925bb783c435320aeb283915ece39da2271
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521989"
---
# <a name="distinguishedfolderid"></a>DistinguishedFolderId

O **elemento DistinguishedFolderId** identifica pastas que podem ser referenciadas pelo nome. Se você não usar esse elemento, deverá usar o [elemento FolderId](folderid.md) para identificar uma pasta. 
  
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
|**ChangeKey** <br/> |Contém uma cadeia de caracteres que identifica uma versão de uma pasta identificada pelo **atributo Id.** Esse atributo é opcional. Use esse atributo para garantir que a versão correta de uma pasta seja usada.  <br/> |
   
#### <a name="id-attribute-values"></a>Valores de atributo Id

|**Valor**|**Descrição**|
|:-----|:-----|
|calendar  <br/> |Representa a pasta Calendário.  <br/> |
|contacts  <br/> |Representa a pasta Contatos.  <br/> |
|deleteditems  <br/> |Representa a pasta Itens Excluídos.  <br/> |
|rascunhos  <br/> |Representa a pasta Rascunhos.  <br/> |
|caixa de entrada  <br/> |Representa a pasta Caixa de Entrada.  <br/> |
|journal  <br/> |Representa a pasta Diário.  <br/> |
|notes  <br/> |Representa a pasta Notes.  <br/> |
|Caixa de saída  <br/> |Representa a pasta Caixa de Saída.  <br/> |
|sentitems  <br/> |Representa a pasta Itens Enviados.  <br/> |
|tarefas  <br/> |Representa a pasta Tarefas.  <br/> |
|msgfolderroot  <br/> |Representa a raiz da pasta de mensagem.  <br/> |
|root  <br/> |Representa a raiz da caixa de correio.  <br/> |
|junkemail  <br/> |Representa a pasta Lixo Eletrônico.  <br/> |
|SearchFolders  <br/> |Representa a pasta Pastas de Pesquisa.  <br/> |
|voicemail  <br/> |Representa a pasta Caixa Postal.  <br/> |
|recoverableitemsroot  <br/> |Representa a pasta raiz de lixeira.  <br/> |
|recoverableitemsdeletions  <br/> |Representa a pasta de exclusões de lixeira.  <br/> |
|recoverableitemsversions  <br/> |Representa a pasta de versões de lixeira.  <br/> |
|recoverableitemspurges  <br/> |Representa a pasta de limpeza de lixeiras.  <br/> |
|archiveroot  <br/> |Representa a pasta de arquivo morto raiz.  <br/> |
|archivemsgfolderroot  <br/> |Representa a pasta de mensagem de arquivo morto raiz.  <br/> |
|archivedeleteditems  <br/> |Representa a pasta de itens excluídos do arquivo morto.  <br/> |
|archiveinbox  <br/> |Representa a pasta Caixa de Entrada de arquivo morto. As versões Exchange a partir do número de com build 15.00.0913.09 incluem esse valor.  <br/> |
|archiverecoverableitemsroot  <br/> |Representa a pasta raiz de itens recuperáveis de arquivo morto.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Representa a pasta de exclusões de itens recuperáveis de arquivo morto.  <br/> |
|archiverecoverableitemsversions  <br/> |Representa a pasta de versões de itens recuperáveis de arquivo morto.  <br/> |
|archiverecoverableitemspurges  <br/> |Representa a pasta de limpeza de itens recuperáveis de arquivo morto.  <br/> |
|syncissues  <br/> |Representa a pasta problemas de sincronização.  <br/> |
|Conflitos  <br/> |Representa a pasta conflitos.  <br/> |
|localfailures  <br/> |Representa a pasta falhas locais.  <br/> |
|serverfailures  <br/> |Representa a pasta falhas do servidor.  <br/> |
|recipientcache  <br/> |Representa a pasta de cache do destinatário.  <br/> |
|quickcontacts  <br/> |Representa a pasta contatos rápidos.  <br/> |
|conversationhistory  <br/> |Representa a pasta histórico da conversa.  <br/> |
|adminauditlogs  <br/> |Representa a pasta logs de auditoria do administrador.  <br/> |
|todosearch  <br/> |Representa a pasta de pesquisa de todo.  <br/> |
|mycontacts  <br/> |Representa a pasta Meus Contatos.  <br/> |
|directory  <br/> |Representa a pasta de diretório.  <br/> |
|imcontactlist  <br/> |Representa a pasta de lista de contatos de IM.  <br/> |
|peopleconnect  <br/> |Representa a pasta de conexão de pessoas.  <br/> |
|favoritos  <br/> |Representa a pasta Favoritos.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Caixa de Correio](mailbox.md) <br/> |Identifica um endereço SMTP principal. Endereços proxy não são permitidos.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |Indica a pasta direcionada para ações de conversa que usam pastas.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Indica a pasta de destino para copiar e mover ações de conversa.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> | Identifica a pasta na qual uma nova pasta ou item é criado.  <br/><br/>Veja a seguir as expressões XPath para este elemento:<br/><br/>  `/CreateItem/ParentFolderId` <br/><br/>`/CreateFolder/ParentFolderId` <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Identifica pastas para pesquisar a operação [FindItem](finditem-operation.md) e a [operação FindFolder.](findfolder-operation.md)  <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |Representa o conjunto de pastas que serão pesquisadas para determinar o conteúdo de uma pasta de pesquisa.  <br/> |
|[FolderIds](folderids.md) <br/> |Contém uma matriz de identificadores de pasta que são usados para identificar pastas para copiar, mover, obter, excluir ou monitorar notificações de eventos.  <br/> |
|[FolderChange](folderchange.md) <br/> |Representa uma coleção de alterações a serem executadas em uma única pasta.  <br/> <br/>Veja a seguir a expressão XPath para este elemento:<br/><br/>`/UpdateFolder/FolderChanges/FolderChange`<br/> |
|[ToFolderId](tofolderid.md) <br/> | Representa a pasta de destino de um item ou pasta copiado ou movido.<br/><br/>Veja a seguir as expressões XPath para este elemento:<br/><br/>`/MoveFolder/ToFolderId`<br/><br/>`/CopyFolder/ToFolderId`<br/><br/>`/MoveItem/ToFolderId`<br/><br/>`/CopyItem/ToFolderId` <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> | Identifica a pasta de destino para operações que atualizem, enviem e criem itens no Exchange store.<br/><br/>Veja a seguir as expressões XPath para este elemento:<br/><br/>`/CreateItem/SavedItemFolderId`<br/><br/>`/UpdateItem/SavedItemFolderId`<br/><br/>`/SendItem/SavedItemFolderId` <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Representa a pasta que contém os itens a sincronizar.  <br/> |
|[UserConfigurationName](userconfigurationname.md) <br/> |Representa o nome de um objeto de configuração do usuário. O nome do objeto de configuração do usuário é o identificador de um objeto de configuração do usuário.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Representa a ID da pasta para a onde os itens de email serão copiados.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Representa a ID da pasta para a onde os itens de email serão movidos.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

Um **DistinguishedFolderId** é resolvido para um **FolderId**. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Criando Pastas (Exchange Web Services)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

