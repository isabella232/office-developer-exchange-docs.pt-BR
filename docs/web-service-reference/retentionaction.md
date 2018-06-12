---
title: RetentionAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3bdf5955-1212-48a1-b3b5-743086866c91
description: O elemento RetentionAction Especifica a ação executada em itens com a marca de retenção.
ms.openlocfilehash: 54a1038f2e56aad66f89522423ccfbd69dc44a80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825215"
---
# <a name="retentionaction"></a>RetentionAction

O elemento **RetentionAction** Especifica a ação executada em itens com a marca de retenção. 
  
```XML
<RetentionAction> None | MoveToDeletedItems | MoveToFolder | DeleteAndAllowRecovery | PermanentlyDelete | MarkAsPastRetentionLimit | MoveToArchive <RetentionAction>
```

 **RetentionActionType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[RetentionPolicyTag](retentionpolicytag.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **RetentionAction** é a ação executada em itens. A lista a seguir contém os valores de texto para o elemento **RetentionAction** . 
  
> **None** - nenhuma ação é executada no item. 
    
> **MoveToDeletedItems** - o item é movido para a pasta de itens excluídos padrão. 
    
> **MoveToFolder** - o item é movido para uma pasta especificada. 
    
> **DeleteAndAllowRecovery** - o item é excluído e colocar no Dumpster de. 
    
> **PermanentlyDelete** - o item é excluído permanentemente da caixa de correio. 
    
> **MarkAsPastRetentionLimit** - o item está marcado como tendo excedeu o limite de tempo de retenção. 
    
> **MoveToArchive** - o item é movido para a caixa de correio de arquivo morto. 
    
## <a name="remarks"></a>Coment�rios

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

