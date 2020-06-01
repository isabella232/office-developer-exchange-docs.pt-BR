---
title: FilterHtmlContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FilterHtmlContent
api_type:
- schema
ms.assetid: 2f9358a0-de1d-4544-9aa0-d9f6519f3b5f
description: O elemento FilterHtmlContent especifica se o conteúdo HTML potencialmente não seguro é filtrado de um item ou anexo.
ms.openlocfilehash: 28e3be86b550c3f330fbb6846b64732b5674304d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462672"
---
# <a name="filterhtmlcontent"></a>FilterHtmlContent

O elemento **FilterHtmlContent** especifica se o conteúdo HTML potencialmente não seguro é filtrado de um item ou anexo. 
  
```xml
<FilterHtmlContent>true or false</FilterHtmlContent>
```

 **boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AttachmentShape](attachmentshape.md) <br/> | Identifica propriedades adicionais para retornar em uma resposta a uma solicitação [GetAttachment](getattachment.md) .  <br/><br/>  A seguir está a expressão XPath para este elemento: <br/> <br/>  `/GetAttachment/AttachmentShape` <br/> |
|[Shape](itemshape.md) <br/> | Identifica as propriedades e o conteúdo do item que serão incluídos em uma resposta GetItem, FindItem ou SyncFolderItems.  <br/> <br/> A seguir estão as expressões XPath para este elemento: <br/> <br/>  `/GetItem/ItemShape`<br/> <br/>  `/FindItem/ItemShape`<br/> <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Valor de texto

Esse elemento pode ser **true** ou **false**. O valor padrão é **false**. Este é um tipo de dados Boolean.
  
## <a name="remarks"></a>Comentários

Este elemento é opcional.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Exchange Server com a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

