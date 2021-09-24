---
title: HasStartTimeChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 04a6968d-7fb5-47ee-b66e-dc99c35dbb63
description: O elemento HasStartTimeChanged especifica se a hora de início de uma reunião foi alterada.
ms.openlocfilehash: 7f04c4d34a081b91adbb0796019e93bc50bfb8ab
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539644"
---
# <a name="hasstarttimechanged"></a>HasStartTimeChanged

O **elemento HasStartTimeChanged** especifica se a hora de início de uma reunião foi alterada. 
  
```XML
<HasStartTimeChanged> true | false </HasStartTimeChanged>
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
|[ChangeHighlights](changehighlights.md) <br/> |Especifica o que mudou entre duas versões de uma mensagem de solicitação de reunião.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** para o **elemento HasStartTimeChanged** indica que a hora de início de uma reunião foi alterada. Um valor **false** indica que a hora de início não foi alterada. 
  
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

