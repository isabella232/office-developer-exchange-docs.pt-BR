---
title: ResolutionSet
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResolutionSet
api_type:
- schema
ms.assetid: 43d5b876-0e87-4414-9b1d-bff1c1ec825c
description: O elemento ResolutionSet contém uma matriz de resoluções para um nome ambíguo.
ms.openlocfilehash: f77b8a94871aa7827c98a3bb15fdf4a3a35c7c55
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521743"
---
# <a name="resolutionset"></a>ResolutionSet

O **elemento ResolutionSet** contém uma matriz de resoluções para um nome ambíguo. 
  
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
|**IndexedPagingOffset** <br/> |Representa o próximo índice que deve ser usado para a próxima solicitação quando você estiver usando um exibição de página indexada.  <br/> |
|**NumeratorOffset** <br/> |Representa o novo valor de numerador a ser usado para a próxima solicitação quando você estiver usando exibições de página fracionada.  <br/> |
|**AbsoluteDenominator** <br/> |Representa o próximo denominador a ser usado para a próxima solicitação quando você estiver usando exibições de página fracionada.  <br/> |
|**IncludesLastItemInRange** <br/> |Esse atributo será true se os resultados atuais contêm o último item na consulta, de forma que a paja adicional não seja necessária.  <br/> |
|**TotalItemsInView** <br/> |Representa o número total de itens no exibição.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Resolução](resolution.md) <br/> |Contém uma única entidade resolvida.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação ResolveNames.  <br/> |
   
## <a name="remarks"></a>Comentários

Um **elemento ResolutionSet** pode conter no máximo 100 entidades resolvidas. 
  
O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
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

