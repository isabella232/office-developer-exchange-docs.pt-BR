---
title: AddBlankTargetToLinks
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 30180298-2501-4369-9b8f-2f7663f02336
description: O elemento AddBlankTargetToLinks especifica que o atributo de destino em links HTML está definido para abrir uma nova janela.
ms.openlocfilehash: c8d7a5973e60e43638472b0da29842ce1caacc98
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543825"
---
# <a name="addblanktargettolinks"></a>AddBlankTargetToLinks

O **elemento AddBlankTargetToLinks** especifica que o atributo de destino em links HTML está definido para abrir uma nova janela. 
  
```XML
<AddBlankTargetToLinks> true | false </AddBlankTargetToLinks>
```

**xs:Boolean**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> | Identifica as propriedades do item e o conteúdo a ser incluído em uma resposta **GetItem,** **FindItem,** **GetConversationItems** ou **SyncFolderItems.**<br/><br/>  Veja a seguir as expressões XPath para este elemento:<br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/>  `/GetConversationItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** para o **elemento AddBlankTargetToLinks** indica que todos os links HTML serão definidos para abrir uma nova janela. Um valor **false** indica que os links HTML serão abertos na janela atual. 
  
## <a name="remarks"></a>Comentários

Esse elemento é opcional.
  
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

