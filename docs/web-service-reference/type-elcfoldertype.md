---
title: Tipo (ElcFolderType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6faad98f-1a92-4373-bde5-dd12af61765f
description: O elemento Type especifica o tipo da pasta usada em uma política de retenção.
ms.openlocfilehash: f679a9237a577d26d4b28e1b25f3e135f7193903
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837804"
---
# <a name="type-elcfoldertype"></a>Tipo (ElcFolderType)

O **tipo** de elemento Especifica o tipo da pasta usada em uma política de retenção. 
  
```XML
<Type> Calendar | Contacts | DeletedItems | Drafts | Inbox | JunkEmail | Journal | Notes | Outbox | SentItems | Tasks | All | ManagedCustomFolder | RssSubscriptions | SyncIssues | ConversationHistory | Personal | RecoverableItems | NonIpmRoot <Type>
```

 **ElcFolderType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[RetentionPolicyTag](retentionpolicytag.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **Type** é o tipo de pasta usado em uma política de retenção. O valor de texto pode ser um dos seguintes valores que representam um tipo de pasta padrão: calendário, contatos, DeletedItems, Rascunhos, caixa de entrada, JunkEmail, diário, anotações, caixa de saída, itens enviados, tarefas, All, ManagedCustomFolder, RssSubscriptions, SyncIssues, ConversationHistory, pessoal, RecoverableItems ou NonIpmRoot 
  
## <a name="remarks"></a>Coment�rios

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |false  <br/> |
   

