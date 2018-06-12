---
title: ArchiveTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c4cb0718-37cd-41aa-86e7-b492c4bb86aa
description: O elemento ArchiveTag Especifica o identificador de retenção da marca archive definir em um item ou pasta.
ms.openlocfilehash: ae9c7d512981af3bf564bcb73a9a27c5c78217fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751203"
---
# <a name="archivetag"></a>ArchiveTag

O elemento **ArchiveTag** Especifica o identificador de retenção da marca archive definir em um item ou pasta. 
  
```XML
<ArchiveTag IsExplicit=""></ArchiveTag>
```

 **RetentionTagType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**IsExplicit** <br/> |Especifica se a política de retenção é definida explicitamente em uma pasta ou um item ou se ela é herdada da pasta pai.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Representa uma pasta que contém principalmente itens de calendário.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato no armazenamento do Exchange.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Representa uma pasta de contatos que está contida em uma caixa de correio.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[Folder](folder.md) <br/> |Define uma pasta para criar, obter, encontre, sincronizar ou atualizar.  <br/> |
|[1.1](item.md) <br/> |Representa um item genérico no armazenamento do Exchange.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem de email do Microsoft Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Representa um item de postagem no armazenamento do Exchange.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Representa uma pasta de pesquisa que está contida em uma caixa de correio.  <br/> |
|[Task](task.md) <br/> |Representa uma tarefa no armazenamento do Exchange.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Representa uma pasta de tarefas que está contida em uma caixa de correio.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto do elemento **ArchiveTag** é um GUID que identifica a política de retenção. 
  
## <a name="remarks"></a>Coment�rios

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

