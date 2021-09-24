---
title: IsMembershipGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0dc3e285-8f49-48ad-b844-37041c0d782b
description: O elemento IsMembershipGroup especifica um valor Boolean que indica se a entidade é um grupo de distribuição ou uma caixa de correio.
ms.openlocfilehash: 111a517a5258a48aada1c7768c908d62f3a47b9e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540976"
---
# <a name="ismembershipgroup"></a>IsMembershipGroup

O **elemento IsMembershipGroup** especifica um valor Boolean que indica se a entidade é um grupo de distribuição ou uma caixa de correio. 
  
```XML
<IsMembershipGroup>true | false</IsMembershipGroup>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SearchableMailbox](searchablemailbox.md) <br/> |Especifica uma caixa de correio retornada de uma **solicitação GetSearchableMailboxes.**  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true para** o **elemento IsMembershipGroup** indica que a entidade é um grupo de distribuição ou uma caixa de correio. Um valor false indica que a entidade não é um grupo de distribuição ou uma caixa de correio. 
  
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

