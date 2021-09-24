---
title: ArchiveTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c4cb0718-37cd-41aa-86e7-b492c4bb86aa
description: O elemento ArchiveTag especifica o identificador de retenção do conjunto de marca de arquivo morto em um item ou pasta.
ms.openlocfilehash: c3545b505dc0596d7465154e0be7d6c758b24ec9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525236"
---
# <a name="archivetag"></a>ArchiveTag

O **elemento ArchiveTag** especifica o identificador de retenção do conjunto de marca de arquivo morto em um item ou pasta. 
  
```XML
<ArchiveTag IsExplicit=""></ArchiveTag>
```

 **RetentionTagType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**IsExplicit** <br/> |Especifica se a política de retenção está explicitamente definida em um item ou pasta ou se ela é herdada de uma pasta pai.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Representa uma pasta que contém principalmente itens de calendário.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um Exchange de calendário.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato no Exchange store.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Representa uma pasta de contatos contida em uma caixa de correio.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[Folder](folder.md) <br/> |Define uma pasta para criar, obter, encontrar, sincronizar ou atualizar.  <br/> |
|[Item](item.md) <br/> |Representa um item genérico no Exchange store.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem Exchange email da Microsoft.  <br/> |
|[Item de postagem](postitem.md) <br/> |Representa um item post no Exchange store.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Representa uma pasta de pesquisa contida em uma caixa de correio.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no Exchange store.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Representa uma pasta de tarefas contida em uma caixa de correio.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento ArchiveTag** é um GUID que identifica a política de retenção. 
  
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

