---
title: ResolutionSet
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolutionSet
api_type:
- schema
ms.assetid: 43d5b876-0e87-4414-9b1d-bff1c1ec825c
description: O elemento ResolutionSet contém uma matriz de resoluções para um nome ambíguo.
ms.openlocfilehash: 483a096a7fcedbabe25758ebcaa31c83405a0ad4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467169"
---
# <a name="resolutionset"></a>ResolutionSet

O elemento **ResolutionSet** contém uma matriz de resoluções para um nome ambíguo. 
  
[ResolveNamesResponse](resolvenamesresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
  
[ResolutionSet](resolutionset.md)
  
```xml
<ResolutionSet IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Resolution/>
</ResolutionSet>
```

 **ArrayOfResolutionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**IndexedPagingOffset** <br/> |Representa o próximo índice que deve ser usado para a próxima solicitação quando você estiver usando um modo de exibição de página indexado.  <br/> |
|**NumeratorOffset** <br/> |Representa o novo valor do numerador a ser usado para a próxima solicitação quando você estiver usando modos de exibição de página de fração.  <br/> |
|**AbsoluteDenominator** <br/> |Representa o próximo denominador a ser usado para a próxima solicitação quando você estiver usando modos de exibição de página de fração.  <br/> |
|**IncludesLastItemInRange** <br/> |Esse atributo será true se os resultados atuais contiverem o último item na consulta, para que a paginação adicional não seja necessária.  <br/> |
|**TotalItemsInView** <br/> |Representa o número total de itens no modo de exibição.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Resolução](resolution.md) <br/> |Contém uma única entidade resolvida.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação ResolveNames.  <br/> |
   
## <a name="remarks"></a>Comentários

Um elemento **ResolutionSet** pode conter um máximo de 100 entidades resolvidas. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[ResolveNames](resolvenames.md)
  
[ResolveNamesResponse](resolvenamesresponse.md)
  
[Operação ResolveNames](resolvenames-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

