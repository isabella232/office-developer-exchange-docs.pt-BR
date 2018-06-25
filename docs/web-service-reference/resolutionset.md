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
description: O elemento ResolutionSet contém uma matriz de resoluções referentes a um nome ambíguo.
ms.openlocfilehash: ad7bd31c85051e8c80aea25aa9e6f2914cf0ad01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825160"
---
# <a name="resolutionset"></a>ResolutionSet

O elemento **ResolutionSet** contém uma matriz de resoluções referentes a um nome ambíguo. 
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**IndexedPagingOffset** <br/> |Representa o próximo índice que deve ser usado para a próxima solicitação quando você estiver usando um modo de exibição de página indexados.  <br/> |
|**NumeratorOffset** <br/> |Representa o novo valor numerador a ser usado para a próxima solicitação quando você estiver usando os modos de exibição de página de fração.  <br/> |
|**AbsoluteDenominator** <br/> |Representa o denominador próximo a ser usado para a próxima solicitação quando você estiver usando os modos de exibição de página de fração.  <br/> |
|**IncludesLastItemInRange** <br/> |Este atributo será true se os resultados atuais contêm o último item na consulta, para que a paginação adicional não é necessária.  <br/> |
|**TotalItemsInView** <br/> |Representa o número total de itens no modo de exibição.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Resolução](resolution.md) <br/> |Contém uma única entidade resolvida.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de ResolveNames.  <br/> |
   
## <a name="remarks"></a>Comentários

Um elemento **ResolutionSet** pode conter no máximo 100 entidades resolvidos. 
  
O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[ResolveNames](resolvenames.md)
  
[ResolveNamesResponse](resolvenamesresponse.md)
  
[Operação ResolveNames](resolvenames-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

