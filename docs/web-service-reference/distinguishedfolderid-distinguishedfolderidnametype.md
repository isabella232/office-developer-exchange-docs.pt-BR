---
title: DistinguishedFolderId (DistinguishedFolderIdNameType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 915b2ee9-8284-4bf6-8995-1fd0785e9e48
description: O elemento DistinguishedFolderId identifica as pastas que podem ser referidas por nome.
ms.openlocfilehash: 1f5b97fc7ee7b93989762c26e4b979a8dfb884be
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751900"
---
# <a name="distinguishedfolderid-distinguishedfolderidnametype"></a>DistinguishedFolderId (DistinguishedFolderIdNameType)

O elemento **DistinguishedFolderId** identifica as pastas que podem ser referidas por nome. 
  
```XML
<DistinguishedFolderId> calendar | contacts | deleteditems | drafts | inbox | journal | notes | outbox | sentitems | tasks | msgfolderroot | publicfoldersroot | root | junkemail | searchfolders | voicemail | recoverableitemsroot | recoverableitemsdeletions | recoverableitemsversions | recoverableitemspurges | archiveroot | archivemsgfolderroot | archivedeleteditems | archiverecoverableitemsroot | archiverecoverableitemsdeletions | archiverecoverableitemsversions | archiverecoverableitemspurges | syncissues | conflicts | localfailures | serverfailures | recipientcache | quickcontacts | conversationhistory | adminauditlogs | todosearch | mycontacts | directory | imcontactlist | peopleconnect</DistinguishedFolderId>
```

 **DistinguishedFolderIdNameType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

None
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Especifica uma pasta genérica.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Especifica uma pasta de calendário.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Especifica uma pasta de contatos.  <br/> |
   
## <a name="text-value"></a>Text value

**Valores de texto do elemento DistinguishedFolderId**

|**Valor**|**Descrição**|
|:-----|:-----|
|calendário  <br/> |Indica a URL da pasta Calendário.  <br/> |
|contatos  <br/> |Indica a URL da pasta Contatos.  <br/> |
|deleteditems  <br/> |Indica a URL da pasta Itens excluídos.  <br/> |
|rascunhos  <br/> |Indica a URL da pasta Rascunhos.  <br/> |
|caixa de entrada  <br/> |Indica a URL da pasta de caixa de entrada.  <br/> |
|diário  <br/> |Indica a URL da pasta diário.  <br/> |
|Observações  <br/> |Indica a URL da pasta anotações.  <br/> |
|caixa de saída  <br/> |Indica a URL da pasta caixa de saída.  <br/> |
|itens enviados  <br/> |Indica a URL da pasta Itens enviados.  <br/> |
|tarefas  <br/> |Indica a URL da pasta tarefas.  <br/> |
|msgfolderroot  <br/> |Indica a URL da pasta raiz de mensagem.  <br/> |
|publicfoldersroot  <br/> |Indica a URL da pasta raiz de pastas públicas.  <br/> |
|root  <br/> |Indica a URL da pasta raiz.  <br/> |
|junkemail  <br/> |Indica a URL da pasta Lixo eletrônico.  <br/> |
|SearchFolders  <br/> |Indica a URL das pastas de pesquisa.  <br/> |
|caixa postal  <br/> |Indica a URL da pasta de caixa postal.  <br/> |
|recoverableitemsroot  <br/> |Indica a URL da pasta itens recuperáveis raiz.  <br/> |
|recoverableitemsdeletions  <br/> |Indica a URL da pasta itens recuperáveis excluídos.  <br/> |
|recoverableitemsversions  <br/> |Indica a URL da pasta de versões de item recuperável.  <br/> |
|recoverableitemspurges  <br/> |Indica a URL da pasta itens recuperáveis removidos.  <br/> |
|archiveroot  <br/> |Indica a URL da pasta de raiz de arquivamento.  <br/> |
|archivemsgfolderroot  <br/> |Indica a URL da pasta de raiz da pasta de mensagem arquivada.  <br/> |
|archivedeleteditems  <br/> |Indica a URL da pasta Itens excluídos arquivados.  <br/> |
|archiverecoverableitemsroot  <br/> |Indica a URL da pasta itens recuperáveis arquivados raiz.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Indica a URL da pasta Itens excluídos de recuperáveis arquivados.  <br/> |
|archiverecoverableitemsversions  <br/> |Indica a URL da pasta itens recuperáveis arquivados versões.  <br/> |
|archiverecoverableitemspurges  <br/> |Indica a URL da pasta itens recuperáveis de removidos arquivados.  <br/> |
|syncissues  <br/> |Indica a URL da pasta de problemas de sincronização.  <br/> |
|conflitos  <br/> |Indica a URL da pasta conflitos.  <br/> |
|localfailures  <br/> |Indica a URL da pasta falhas locais.  <br/> |
|serverfailures  <br/> |Indica a URL da pasta de falhas do servidor.  <br/> |
|recipientcache  <br/> |Indica a URL da pasta de cache de destinatários.  <br/> |
|QuickContacts  <br/> |Indica a URL da pasta Contatos rápidos.  <br/> |
|conversationhistory  <br/> |Indica a URL da pasta de histórico da conversa.  <br/> |
|adminauditlogs  <br/> |Indica a URL da pasta de log de auditoria administrativas.  <br/> |
|todosearch  <br/> |Indica a URL da pasta de pesquisa de tarefas pendentes.  <br/> |
|mycontacts  <br/> |Indica a URL da minha pasta de contatos.  <br/> |
|diretório  <br/> |Indica uma URL da pasta do diretório.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

