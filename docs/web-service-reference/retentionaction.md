---
title: RetentionAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3bdf5955-1212-48a1-b3b5-743086866c91
description: O elemento RetentionAction especifica a ação executada em itens com a marca de retenção.
ms.openlocfilehash: ecea4326f0e50460635966991cd55badf8946993
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517942"
---
# <a name="retentionaction"></a>RetentionAction

O **elemento RetentionAction** especifica a ação executada em itens com a marca de retenção. 
  
```XML
<RetentionAction> None | MoveToDeletedItems | MoveToFolder | DeleteAndAllowRecovery | PermanentlyDelete | MarkAsPastRetentionLimit | MoveToArchive <RetentionAction>
```

 **RetentionActionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[RetentionPolicyTag](retentionpolicytag.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento RetentionAction** é a ação executada em itens. A lista a seguir contém os valores de texto do **elemento RetentionAction.** 
  
> **Nenhum** - Nenhuma ação é executada no item. 
    
> **MoveToDeletedItems** - O item é movido para a pasta itens excluídos padrão. 
    
> **MoveToFolder** - O item é movido para uma pasta especificada. 
    
> **DeleteAndAllowRecovery** - O item é excluído e colocado no Dumpster. 
    
> **PermanentlyDelete** - O item é excluído permanentemente da caixa de correio. 
    
> **MarkAsPastRetentionLimit** - O item está marcado como tendo excedido o limite de tempo de retenção. 
    
> **MoveToArchive** - O item é movido para a caixa de correio de arquivo morto. 
    
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

