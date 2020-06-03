---
title: RootFolder (FindItemResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 187e009f-efaa-42a8-8962-329a645213ab
description: O elemento RootFolder contém os resultados de uma pesquisa de uma única pasta raiz durante uma operação FindItem.
ms.openlocfilehash: 3bbab325dff26139739c50ef519b215aea620a0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457127"
---
# <a name="rootfolder-finditemresponsemessage"></a>RootFolder (FindItemResponseMessage)

O elemento **RootFolder** contém os resultados de uma pesquisa de uma única pasta raiz durante uma [operação FindItem](finditem-operation.md).
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Items/>
   <Groups/>
</RootFolder>
```

 **FindItemParentType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**IndexedPagingOffset** <br/> |Representa o próximo índice que deve ser usado para a próxima solicitação ao usar um modo de exibição de paginação indexado.  <br/> |
|**NumeratorOffset** <br/> |Representa o novo valor do numerador a ser usado para a próxima solicitação ao usar as exibições da página de fração.  <br/> |
|**AbsoluteDenominator** <br/> |Representa o próximo denominador a ser usado para a próxima solicitação ao fazer paginação fracionária.  <br/> |
|**IncludesLastItemInRange** <br/> |Indica se os resultados atuais contêm o último item da consulta, de modo que a paginação adicional não será necessária.  <br/> |
|**TotalItemsInView** <br/> |Representa o número total de itens que passam a restrição. Em uma [operação FindItem](finditem-operation.md)agrupada, o atributo **TotalItemsInView** retorna o número total de itens no modo de exibição mais o número total de grupos.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Itens](items.md) <br/> |Contém uma matriz de itens encontrados que têm os critérios de pesquisa identificados na solicitação de [operação FindItem](finditem-operation.md) .  <br/> |
|[Grupos](groups.md) <br/> |Contém uma coleção de grupos encontrados que têm os critérios de pesquisa e agregação identificados na solicitação de [operação FindItem](finditem-operation.md) .  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação FindItem](finditem-operation.md) .  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Exchange Server com a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindItem](finditem-operation.md)
  
[IndexedPagingOffset](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IndexedPagingOffset.aspx)
  
[NumeratorOffset](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.NumeratorOffset.aspx)
  
[AbsoluteDenominator](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.AbsoluteDenominator.aspx)
  
[IncludesLastItemInRange](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IncludesLastItemInRange.aspx)
  
[TotalItemsInView](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.TotalItemsInView.aspx)


[Localizar itens](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

