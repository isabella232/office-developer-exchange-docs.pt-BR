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
description: O elemento RootFolder contém os resultados de uma pesquisa de uma pasta raiz única durante uma operação FindItem.
ms.openlocfilehash: ea17369ef4efc4112a738b430c8f0dbab3886341
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825254"
---
# <a name="rootfolder-finditemresponsemessage"></a>RootFolder (FindItemResponseMessage)

O elemento **RootFolder** contém os resultados de uma pesquisa de uma pasta raiz única durante uma [operação FindItem](finditem-operation.md).
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Items/>
   <Groups/>
</RootFolder>
```

 **FindItemParentType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**IndexedPagingOffset** <br/> |Representa o próximo índice que deve ser usado para a próxima solicitação ao usar o modo de exibição indexada paginação.  <br/> |
|**NumeratorOffset** <br/> |Representa o novo valor numerador usada para a próxima solicitação quando usar exibições de página de fração.  <br/> |
|**AbsoluteDenominator** <br/> |Representa o denominador próximo a ser usado para a próxima solicitação ao fazer a paginação fracional.  <br/> |
|**IncludesLastItemInRange** <br/> |Indica se os resultados atuais contêm o último item na consulta, de forma que não seja necessário paginação ainda mais.  <br/> |
|**TotalItemsInView** <br/> |Representa o número total de itens que passam a restrição. Em uma [operação FindItem](finditem-operation.md)agrupada, o atributo **TotalItemsInView** retorna o número total de itens no modo de exibição mais o número total de grupos.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Items](items.md) <br/> |Contém uma matriz de itens encontrados com os critérios de pesquisa identificados na solicitação de [operação FindItem](finditem-operation.md) .  <br/> |
|[Grupos](groups.md) <br/> |Contém uma coleção dos grupos encontrados que tenham os critérios de pesquisa e a agregação de lista segura identificados na solicitação de [operação FindItem](finditem-operation.md) .  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação FindItem](finditem-operation.md) .  <br/> |
   
## <a name="remarks"></a>Coment�rios

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server com a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação FindItem](finditem-operation.md)
  
[IndexedPagingOffset](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IndexedPagingOffset.aspx)
  
[NumeratorOffset](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.NumeratorOffset.aspx)
  
[AbsoluteDenominator](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.AbsoluteDenominator.aspx)
  
[IncludesLastItemInRange](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IncludesLastItemInRange.aspx)
  
[TotalItemsInView](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.TotalItemsInView.aspx)


[Localizando itens](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

