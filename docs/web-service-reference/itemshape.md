---
title: Shape
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemShape
api_type:
- schema
ms.assetid: c5604161-bbc0-40bc-ad75-ff7e837d745f
description: O elemento doshape identifica um conjunto de propriedades para retornar em uma operação GetItem, FindItem ou uma resposta de operação SyncFolderItems.
ms.openlocfilehash: ffb666ee331b55a4f04cad076c705e4bec980e03
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458121"
---
# <a name="itemshape"></a>Shape

O elemento **doshape** identifica um conjunto de propriedades para retornar em uma [operação GetItem](getitem-operation.md), [FindItem](finditem-operation.md)ou uma resposta de [operação SyncFolderItems](syncfolderitems-operation.md) . 
  
```XML
<ItemShape>
   <BaseShape/>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <ConvertHtmlCodePageToUTF8/>
   <AdditionalProperties/>
</ItemShape>
```

 **ItemResponseShapeType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[BaseShape](baseshape.md) <br/> |Identifica a configuração básica de propriedades a serem retornadas em uma resposta de item ou pasta.  <br/> |
|[IncludeMimeContent](includemimecontent.md) <br/> |Especifica se o conteúdo MIME (Multipurpose Internet Mail Extensions) de um item é retornado na resposta.  <br/> |
|[BodyType](bodytype.md) <br/> |Identifica como o corpo de texto é formatado na resposta.  <br/> |
|[ConvertHtmlCodePageToUTF8](converthtmlcodepagetoutf8.md) <br/> |Indica se o corpo de HTML do item é convertido em UTF8.  <br/> |
|[FilterHtmlContent](filterhtmlcontent.md) <br/> |Especifica se a filtragem de conteúdo HTML está habilitada.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |Identifica propriedades adicionais a serem retornadas em uma resposta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetItem](getitem.md) <br/> |Define uma solicitação para recuperar itens de uma caixa de correio no repositório do Exchange.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/GetItem` <br/> |
|[FindItem](finditem.md) <br/> |Define uma solicitação para localizar todos os itens contidos em uma pasta.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/FindItem` <br/> |
|[SyncFolderItems](syncfolderitems.md) <br/> |Define uma solicitação para sincronizar itens em uma pasta do repositório do Exchange.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/SyncFolderItems` <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetItem](getitem-operation.md)
  
[Operação FindItem](finditem-operation.md)
  
[Operação SyncFolderItems](syncfolderitems-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

