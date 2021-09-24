---
title: HasAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: de152be6-fc2f-48bc-a05d-1211935da20a
description: O elemento HasAttachment especifica um valor Boolean para indicar se o item tem anexos.
ms.openlocfilehash: c3d153e86a9d170c69e74bdc08a3bdedfa5e1220
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516794"
---
# <a name="hasattachment"></a>HasAttachment

O **elemento HasAttachment** especifica um valor Boolean para indicar se o item tem anexos. 
  
```XML
<HasAttachment> true | false </HasAttachment
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
|[SearchPreviewItem](searchpreviewitem.md) <br/> |Especifica os primeiros 256 caracteres de um item de caixa de correio para visualização sem abrir o item.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** para o **elemento HasAttachment** indica que o item tem um anexo. Um valor **false** indica que o item não tem um anexo. 
  
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

