---
title: ImListMigrationCompleted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6eed9502-5d9e-4345-ba23-3582ff487147
description: O elemento ImListMigrationCompleted indica se o armazenamento do Exchange contém os itens de mensagens instantâneos usados por clientes de mensagens instantâneas.
ms.openlocfilehash: 25f1b583b354a71958fbc8052c492726dc0eb7db
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823893"
---
# <a name="imlistmigrationcompleted"></a>ImListMigrationCompleted

O elemento **ImListMigrationCompleted** indica se o armazenamento do Exchange contém a itens usados por clientes de mensagens instantâneas de mensagens instantâneas. 
  
```XML
<ImListMigrationCompleted>true | false</ImListMigrationCompleted>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[SetImListMigrationCompleted](setimlistmigrationcompleted.md)
  
## <a name="text-value"></a>Text value

Um valor de texto de **true** para o elemento **ImListMigrationCompleted** indica que os contatos de mensagens instantâneas repositório ter sido migrado para o Exchange armazenam. Um valor **false** indica que o repositório de contatos de mensagem instantânea não tenha sido migrado. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

