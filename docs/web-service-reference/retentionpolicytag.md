---
title: RetentionPolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f46679d0-9236-41e2-8624-72300079c67c
description: O elemento RetentionPolicyTag especifica a política de retenção de um item de caixa de correio.
ms.openlocfilehash: 58ca3016bed0be625b213a57e5ead1b38a301bfa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524543"
---
# <a name="retentionpolicytag"></a>RetentionPolicyTag

O **elemento RetentionPolicyTag** especifica a política de retenção de um item de caixa de correio. 
  
```XML
<RetentionPolicyTag>
   <DisplayName/>
   <RetentionId/>
   <RetentionPeriod/>
   <Type/>
   <RetentionAction/>
   <Description/>
   <IsVisible/>
   <OptedInto/>
   <IsArchive/>
</RetentionPolicyTag>
```

 **RetentionPolicyTagType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[DisplayName (cadeia de caracteres)](displayname-string.md)  |  [RetentionId](retentionid.md)  |  [RetentionPeriod](retentionperiod.md)  |  [Tipo (ElcFolderType)](type-elcfoldertype.md)  |  [RetentionAction](retentionaction.md)  |  [Descrição](description.md)  |  [IsVisible](isvisible.md)  |  [OptedInto](optedinto.md)  |  [IsArchive](isarchive.md)
  
### <a name="parent-elements"></a>Elementos pai

[RetentionPolicyTags](retentionpolicytags.md)
  
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
   

