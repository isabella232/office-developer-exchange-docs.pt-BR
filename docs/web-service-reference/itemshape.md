---
title: ItemShape
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ItemShape
api_type:
- schema
ms.assetid: c5604161-bbc0-40bc-ad75-ff7e837d745f
description: O elemento ItemShape identifica um conjunto de propriedades a ser retornada em uma operação GetItem, operação FindItem ou resposta de operação SyncFolderItems.
ms.openlocfilehash: d6cc1efc85a8a22e12f2a3616fe949b72b3bba33
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519391"
---
# <a name="itemshape"></a>ItemShape

O **elemento ItemShape** identifica um conjunto de propriedades a ser retornada em uma operação [GetItem,](getitem-operation.md)operação [FindItem](finditem-operation.md)ou resposta de operação [SyncFolderItems.](syncfolderitems-operation.md) 
  
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
|[BaseShape](baseshape.md) <br/> |Identifica a configuração básica das propriedades a ser retornada em uma resposta de item ou pasta.  <br/> |
|[IncludeMimeContent](includemimecontent.md) <br/> |Especifica se o conteúdo mime (Extensões de Email da Internet) multipropósito de um item é retornado na resposta.  <br/> |
|[BodyType](bodytype.md) <br/> |Identifica como o texto do corpo é formatado na resposta.  <br/> |
|[ConvertHtmlCodePageToUTF8](converthtmlcodepagetoutf8.md) <br/> |Indica se o corpo HTML do item é convertido em UTF8.  <br/> |
|[FilterHtmlContent](filterhtmlcontent.md) <br/> |Especifica se a filtragem de conteúdo HTML está habilitada.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |Identifica propriedades adicionais para retornar em uma resposta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetItem](getitem.md) <br/> |Define uma solicitação para recuperar itens de uma caixa de correio no Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/GetItem` <br/> |
|[FindItem](finditem.md) <br/> |Define uma solicitação para encontrar todos os itens contidos em uma pasta.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/FindItem` <br/> |
|[SyncFolderItems](syncfolderitems.md) <br/> |Define uma solicitação para sincronizar itens em uma pasta Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/SyncFolderItems` <br/> |
   
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

