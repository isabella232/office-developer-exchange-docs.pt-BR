---
title: ImListMigrationCompleted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 6eed9502-5d9e-4345-ba23-3582ff487147
description: O elemento ImListMigrationCompleted indica se o armazenamento Exchange contém os itens de mensagens instantâneas usados pelos clientes de mensagens instantâneas.
ms.openlocfilehash: b55f3d72259897d7bdf46b351421b0148a41b93e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514610"
---
# <a name="imlistmigrationcompleted"></a>ImListMigrationCompleted

O **elemento ImListMigrationCompleted** indica se o armazenamento Exchange contém os itens de mensagens instantâneas usados por clientes de mensagens instantâneas. 
  
```XML
<ImListMigrationCompleted>true | false</ImListMigrationCompleted>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[SetImListMigrationCompleted](setimlistmigrationcompleted.md)
  
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** para o elemento **ImListMigrationCompleted** indica que o armazenamento de contatos de mensagens instantâneas foi migrado para o Exchange store. Um valor **false** indica que o armazenamento de contatos de mensagem instantânea não foi migrado. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

