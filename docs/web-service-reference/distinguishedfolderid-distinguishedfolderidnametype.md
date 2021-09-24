---
title: DistinguishedFolderId (DistinguishedFolderIdNameType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 915b2ee9-8284-4bf6-8995-1fd0785e9e48
description: O elemento DistinguishedFolderId identifica pastas que podem ser referenciadas pelo nome.
ms.openlocfilehash: 23d1dead5a97fe8b2ceb29235f4b784f667d2ee1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526437"
---
# <a name="distinguishedfolderid-distinguishedfolderidnametype"></a>DistinguishedFolderId (DistinguishedFolderIdNameType)

O **elemento DistinguishedFolderId** identifica pastas que podem ser referenciadas pelo nome. 
  
```XML
<DistinguishedFolderId> calendar | contacts | deleteditems | drafts | inbox | journal | notes | outbox | sentitems | tasks | msgfolderroot | publicfoldersroot | root | junkemail | searchfolders | voicemail | recoverableitemsroot | recoverableitemsdeletions | recoverableitemsversions | recoverableitemspurges | archiveroot | archivemsgfolderroot | archivedeleteditems | archiverecoverableitemsroot | archiverecoverableitemsdeletions | archiverecoverableitemsversions | archiverecoverableitemspurges | syncissues | conflicts | localfailures | serverfailures | recipientcache | quickcontacts | conversationhistory | adminauditlogs | todosearch | mycontacts | directory | imcontactlist | peopleconnect</DistinguishedFolderId>
```

 **DistinguishedFolderIdNameType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Especifica uma pasta genérica.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Especifica uma pasta de calendário.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Especifica uma pasta de contatos.  <br/> |
   
## <a name="text-value"></a>Valor de texto

**Valores de texto do elemento DistinguishedFolderId**

|**Valor**|**Descrição**|
|:-----|:-----|
|calendar  <br/> |Indica a URL da pasta de calendário.  <br/> |
|contacts  <br/> |Indica a URL da pasta de contatos.  <br/> |
|deleteditems  <br/> |Indica a URL da pasta de itens excluídos.  <br/> |
|rascunhos  <br/> |Indica a URL da pasta rascunhos.  <br/> |
|caixa de entrada  <br/> |Indica a URL da pasta de caixa de entrada.  <br/> |
|journal  <br/> |Indica a URL da pasta de diário.  <br/> |
|notes  <br/> |Indica a URL da pasta de anotações.  <br/> |
|Caixa de saída  <br/> |Indica a URL da pasta de caixa de saída.  <br/> |
|sentitems  <br/> |Indica a URL da pasta de itens enviados.  <br/> |
|tarefas  <br/> |Indica a URL da pasta de tarefas.  <br/> |
|msgfolderroot  <br/> |Indica a URL da pasta raiz da mensagem.  <br/> |
|publicfoldersroot  <br/> |Indica a URL da pasta raiz de pastas públicas.  <br/> |
|root  <br/> |Indica a URL da pasta raiz.  <br/> |
|junkemail  <br/> |Indica a URL da pasta lixo eletrônico.  <br/> |
|SearchFolders  <br/> |Indica a URL das pastas de pesquisa.  <br/> |
|voicemail  <br/> |Indica a URL da pasta de caixa postal.  <br/> |
|recoverableitemsroot  <br/> |Indica a URL da pasta raiz de itens recuperáveis.  <br/> |
|recoverableitemsdeletions  <br/> |Indica a URL da pasta de itens recuperáveis excluídos.  <br/> |
|recoverableitemsversions  <br/> |Indica a URL da pasta de versões do item recuperável.  <br/> |
|recoverableitemspurges  <br/> |Indica a URL da pasta de itens recuperáveis limpos.  <br/> |
|archiveroot  <br/> |Indica a URL da pasta raiz de arquivo morto.  <br/> |
|archivemsgfolderroot  <br/> |Indica a URL da pasta raiz da pasta de mensagem arquivada.  <br/> |
|archivedeleteditems  <br/> |Indica a URL da pasta de itens excluídos arquivados.  <br/> |
|archiverecoverableitemsroot  <br/> |Indica a URL da pasta raiz de itens recuperáveis arquivados.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Indica a URL da pasta de itens excluídos recuperáveis arquivados.  <br/> |
|archiverecoverableitemsversions  <br/> |Indica a URL da pasta de versões de itens recuperáveis arquivados.  <br/> |
|archiverecoverableitemspurges  <br/> |Indica a URL da pasta de itens recuperáveis arquivados.  <br/> |
|syncissues  <br/> |Indica a URL da pasta problemas de sincronização.  <br/> |
|Conflitos  <br/> |Indica a URL da pasta conflitos.  <br/> |
|localfailures  <br/> |Indica a URL da pasta de falhas locais.  <br/> |
|serverfailures  <br/> |Indica a URL da pasta falhas do servidor.  <br/> |
|recipientcache  <br/> |Indica a URL da pasta de cache do destinatário.  <br/> |
|quickcontacts  <br/> |Indica a URL da pasta contatos rápidos.  <br/> |
|conversationhistory  <br/> |Indica a URL da pasta histórico da conversa.  <br/> |
|adminauditlogs  <br/> |Indica a URL da pasta de log de auditoria administrativa.  <br/> |
|todosearch  <br/> |Indica a URL da pasta de pesquisa a fazer.  <br/> |
|mycontacts  <br/> |Indica a URL da pasta meus contatos.  <br/> |
|directory  <br/> |Indica uma URL da pasta de diretório.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Tipo de esquema  <br/> |
|Arquivo de validação  <br/> |types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

