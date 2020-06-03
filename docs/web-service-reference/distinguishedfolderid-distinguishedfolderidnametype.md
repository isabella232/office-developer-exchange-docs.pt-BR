---
title: DistinguishedFolderId (DistinguishedFolderIdNameType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 915b2ee9-8284-4bf6-8995-1fd0785e9e48
description: O elemento DistinguishedFolderId identifica pastas que podem ser referenciadas por nome.
ms.openlocfilehash: ac239ec63f78322f6c82ab4be269d6fe4380dd8d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456189"
---
# <a name="distinguishedfolderid-distinguishedfolderidnametype"></a>DistinguishedFolderId (DistinguishedFolderIdNameType)

O elemento **DistinguishedFolderId** identifica pastas que podem ser referenciadas por nome. 
  
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
|calendário  <br/> |Indica a URL da pasta do calendário.  <br/> |
|contacts  <br/> |Indica a URL da pasta contatos.  <br/> |
|deleteditems  <br/> |Indica a URL da pasta itens excluídos.  <br/> |
|rascunhos  <br/> |Indica a URL da pasta Rascunhos.  <br/> |
|caixa de entrada  <br/> |Indica a URL da pasta caixa de entrada.  <br/> |
|diário  <br/> |Indica a URL da pasta do diário.  <br/> |
|notes  <br/> |Indica a URL da pasta anotações.  <br/> |
|Caixa de saída  <br/> |Indica a URL da pasta de saída.  <br/> |
|sentitems  <br/> |Indica a URL da pasta Itens enviados.  <br/> |
|tarefas  <br/> |Indica a URL da pasta tarefas.  <br/> |
|msgfolderroot  <br/> |Indica a URL da pasta raiz da mensagem.  <br/> |
|publicfoldersroot  <br/> |Indica a URL da pasta raiz de pastas públicas.  <br/> |
|root  <br/> |Indica a URL da pasta raiz.  <br/> |
|junkemail  <br/> |Indica a URL da pasta lixo eletrônico.  <br/> |
|SearchFolders  <br/> |Indica a URL das pastas de pesquisa.  <br/> |
|postal  <br/> |Indica a URL da pasta de email de voz.  <br/> |
|recoverableitemsroot  <br/> |Indica a URL da pasta raiz de itens recuperáveis.  <br/> |
|recoverableitemsdeletions  <br/> |Indica a URL da pasta itens recuperáveis excluídos.  <br/> |
|recoverableitemsversions  <br/> |Indica a URL da pasta de versões de Item recuperável.  <br/> |
|recoverableitemspurges  <br/> |Indica a URL da pasta itens recuperáveis descartados.  <br/> |
|archiveroot  <br/> |Indica a URL da pasta raiz de arquivo morto.  <br/> |
|archivemsgfolderroot  <br/> |Indica a URL da pasta raiz da pasta de mensagens arquivadas.  <br/> |
|archivedeleteditems  <br/> |Indica a URL da pasta itens excluídos arquivados.  <br/> |
|archiverecoverableitemsroot  <br/> |Indica a URL da pasta raiz de itens recuperáveis arquivados.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Indica a URL da pasta itens excluídos recuperados arquivados.  <br/> |
|archiverecoverableitemsversions  <br/> |Indica a URL da pasta de versões de itens recuperáveis arquivados.  <br/> |
|archiverecoverableitemspurges  <br/> |Indica a URL da pasta de itens recuperáveis excluídos arquivados.  <br/> |
|syncissues  <br/> |Indica a URL da pasta problemas de sincronização.  <br/> |
|Conflitos  <br/> |Indica a URL da pasta de conflitos.  <br/> |
|localfailures  <br/> |Indica a URL da pasta falhas locais.  <br/> |
|serverfailures  <br/> |Indica a URL da pasta falhas do servidor.  <br/> |
|recipientcache  <br/> |Indica a URL da pasta de cache de destinatários.  <br/> |
|quickcontacts  <br/> |Indica a URL da pasta Contatos rápidos.  <br/> |
|conversationhistory  <br/> |Indica a URL da pasta de histórico de conversas.  <br/> |
|adminauditlogs  <br/> |Indica a URL da pasta de log de auditoria administrativa.  <br/> |
|todosearch  <br/> |Indica a URL da pesquisa de tarefas pendentes.  <br/> |
|MyContacts  <br/> |Indica a URL da pasta meus contatos.  <br/> |
|Directory  <br/> |Indica uma URL da pasta de diretório.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

