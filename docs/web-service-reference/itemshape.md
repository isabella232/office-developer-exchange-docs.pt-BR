---
title: ItemShape
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
description: O elemento ItemShape identifica um conjunto de propriedades para retornar em uma operação de GetItem, operação FindItem ou resposta de operação SyncFolderItems.
ms.openlocfilehash: 95174a85a8fa05cb2612e1289d46c8db32b6e052
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824191"
---
# <a name="itemshape"></a>ItemShape

O elemento **ItemShape** identifica um conjunto de propriedades para retornar em uma resposta de [operação GetItem](getitem-operation.md), [operação FindItem](finditem-operation.md)ou [SyncFolderItems operação](syncfolderitems-operation.md) . 
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[BaseShape](baseshape.md) <br/> |Identifica a configuração básica de propriedades para retornar em uma resposta de item ou uma pasta.  <br/> |
|[IncludeMimeContent](includemimecontent.md) <br/> |Especifica se o conteúdo de email extensões MIME (Multipurpose Internet) de um item é retornado na resposta.  <br/> |
|[BodyType](bodytype.md) <br/> |Identifica como o corpo de texto é formatado na resposta.  <br/> |
|[ConvertHtmlCodePageToUTF8](converthtmlcodepagetoutf8.md) <br/> |Indica se o item do corpo em HTML é convertido em UTF8.  <br/> |
|[FilterHtmlContent](filterhtmlcontent.md) <br/> |Especifica se a filtragem de conteúdo de HTML está habilitado.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |Identifica as propriedades adicionais para retornar em uma resposta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetItem](getitem.md) <br/> |Define uma solicitação para recuperar itens de uma caixa de correio no armazenamento do Exchange.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/GetItem` <br/> |
|[FindItem](finditem.md) <br/> |Define uma solicitação para localizar todos os itens que estão contidos em uma pasta.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/FindItem` <br/> |
|[SyncFolderItems](syncfolderitems.md) <br/> |Define uma solicitação para sincronizar os itens em uma pasta de repositório do Exchange.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/SyncFolderItems` <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação GetItem](getitem-operation.md)
  
[Operação FindItem](finditem-operation.md)
  
[Operação SyncFolderItems](syncfolderitems-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

