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
description: O elemento DistinguishedFolderId identifica as pastas que podem ser referidas por nome. Se você não usar esse elemento, você deve usar o elemento FolderId para identificar uma pasta.
ms.openlocfilehash: 834166be3d882fa8c0533cfcc2999600430b82ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751902"
---
# <a name="distinguishedfolderid"></a>DistinguishedFolderId

O elemento **DistinguishedFolderId** identifica as pastas que podem ser referidas por nome. Se você não usar esse elemento, você deve usar o elemento [FolderId](folderid.md) para identificar uma pasta. 
  
```XML
<DistinguishedFolderId Id="" ChangeKey="">
   <Mailbox/>
</DistinguishedFolderId>
```

 **DistinguishedFolderIdType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**ID de** <br/> |Contém uma cadeia de caracteres que identifica uma pasta padrão. Este atributo é necessário.  <br/> |
|**ChangeKey** <br/> |Contém uma cadeia de caracteres que identifica uma versão de uma pasta que é identificada pelo atributo **Id** . Este atributo é opcional. Use este atributo para certificar-se de que a versão correta de uma pasta é usada.  <br/> |
   
#### <a name="id-attribute-values"></a>Valores do atributo ID

|**Valor**|**Descrição**|
|:-----|:-----|
|calendário  <br/> |Representa a pasta de calendário.  <br/> |
|contatos  <br/> |Representa a pasta de contatos.  <br/> |
|deleteditems  <br/> |Representa a pasta Itens excluídos.  <br/> |
|rascunhos  <br/> |Representa a pasta Rascunhos.  <br/> |
|caixa de entrada  <br/> |Representa a pasta de caixa de entrada.  <br/> |
|diário  <br/> |Representa a pasta diário.  <br/> |
|Observações  <br/> |Representa a pasta anotações.  <br/> |
|caixa de saída  <br/> |Representa a pasta caixa de saída.  <br/> |
|itens enviados  <br/> |Representa a pasta Itens enviados.  <br/> |
|tarefas  <br/> |Representa a pasta tarefas.  <br/> |
|msgfolderroot  <br/> |Representa a raiz da pasta de mensagem.  <br/> |
|root  <br/> |Representa a raiz da caixa de correio.  <br/> |
|junkemail  <br/> |Representa a pasta Lixo eletrônico.  <br/> |
|SearchFolders  <br/> |Representa a pasta de pastas de pesquisa.  <br/> |
|caixa postal  <br/> |Representa a pasta de caixa postal.  <br/> |
|recoverableitemsroot  <br/> |Representa o dumpster pasta raiz.  <br/> |
|recoverableitemsdeletions  <br/> |Representa o dumpster pasta exclusões.  <br/> |
|recoverableitemsversions  <br/> |Representa o dumpster pasta de versões.  <br/> |
|recoverableitemspurges  <br/> |Representa o dumpster limpa a pasta.  <br/> |
|archiveroot  <br/> |Representa a pasta raiz de arquivamento.  <br/> |
|archivemsgfolderroot  <br/> |Representa a pasta raiz de mensagem de arquivo morto.  <br/> |
|archivedeleteditems  <br/> |Representa a pasta de itens excluído de arquivamento.  <br/> |
|archiveinbox  <br/> |Representa o pasta caixa de entrada de arquivo morto. Versões do Exchange, começando com o número de compilação 15.00.0913.09 incluem esse valor.  <br/> |
|archiverecoverableitemsroot  <br/> |Representa a pasta de raiz de itens recuperáveis de arquivamento.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Representa a pasta de exclusões de itens recuperáveis de arquivamento.  <br/> |
|archiverecoverableitemsversions  <br/> |Representa a pasta de versões de itens recuperáveis de arquivamento.  <br/> |
|archiverecoverableitemspurges  <br/> |Representa a pasta de limpezas de itens recuperáveis de arquivamento.  <br/> |
|syncissues  <br/> |Representa a pasta de problemas de sincronização.  <br/> |
|conflitos  <br/> |Representa a pasta conflitos.  <br/> |
|localfailures  <br/> |Representa a pasta falhas locais.  <br/> |
|serverfailures  <br/> |Representa a pasta de falhas do servidor.  <br/> |
|recipientcache  <br/> |Representa a pasta do cache de destinatários.  <br/> |
|QuickContacts  <br/> |Representa a pasta Contatos rápidos.  <br/> |
|conversationhistory  <br/> |Representa a pasta Histórico da conversa.  <br/> |
|adminauditlogs  <br/> |Representa a pasta de logs de auditoria do administrador.  <br/> |
|todosearch  <br/> |Representa a pasta de pesquisa de tarefas pendentes.  <br/> |
|mycontacts  <br/> |Representa a pasta Meus contatos.  <br/> |
|diretório  <br/> |Representa a pasta de diretório.  <br/> |
|imcontactlist  <br/> |Representa a pasta de lista de contatos de mensagens Instantâneas.  <br/> |
|peopleconnect  <br/> |Representa as pessoas se conectar a pasta.  <br/> |
|favoritos  <br/> |Representa a pasta Favoritos.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Caixa de correio](mailbox.md) <br/> |Identifica um endereço SMTP principal. Endereços de proxy não são permitidos.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |Indica a pasta que está programada para ações de conversa que usam pastas.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Indica a pasta de destino para cópia e mover ações de conversa.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> | Identifica a pasta em que uma nova pasta ou um item é criado.  <br/><br/>A seguir estão as expressões XPath para esse elemento:<br/><br/>  `/CreateItem/ParentFolderId` <br/><br/>`/CreateFolder/ParentFolderId` <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Identifica as pastas para procurar a [operação FindItem](finditem-operation.md) e a [operação FindFolder](findfolder-operation.md).  <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |Representa a coleção de pastas que será pesquisada para determinar o conteúdo de uma pasta de pesquisa.  <br/> |
|[FolderIds](folderids.md) <br/> |Contém uma matriz de identificadores de pasta que são usados para identificar pastas para copiar, mover, obter, excluir ou monitorar as notificações de eventos.  <br/> |
|[FolderChange](folderchange.md) <br/> |Representa uma coleção de alterações a serem realizadas em uma única pasta.  <br/> <br/>Este é a expressão XPath para esse elemento:<br/><br/>`/UpdateFolder/FolderChanges/FolderChange`<br/> |
|[ToFolderId](tofolderid.md) <br/> | Representa a pasta de destino para um item movido ou copiada ou uma pasta.<br/><br/>A seguir estão as expressões XPath para esse elemento:<br/><br/>`/MoveFolder/ToFolderId`<br/><br/>`/CopyFolder/ToFolderId`<br/><br/>`/MoveItem/ToFolderId`<br/><br/>`/CopyItem/ToFolderId` <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> | Identifica a pasta de destino para operações de atualização, enviar e crie itens no armazenamento do Exchange.<br/><br/>A seguir estão as expressões XPath para esse elemento:<br/><br/>`/CreateItem/SavedItemFolderId`<br/><br/>`/UpdateItem/SavedItemFolderId`<br/><br/>`/SendItem/SavedItemFolderId` <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Representa a pasta que contém os itens a serem sincronizados.  <br/> |
|[UserConfigurationName](userconfigurationname.md) <br/> |Representa o nome de um objeto de configuração do usuário. O nome de objeto de configuração do usuário é o identificador de um objeto de configuração do usuário.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Representa o ID da pasta que serão copiadas para itens de email.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Representa o ID da pasta esse email itens serão movidos para.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

Um **DistinguishedFolderId** resolve um **FolderId**. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Criação de pastas (serviços Web do Exchange)](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

