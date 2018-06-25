---
title: DLExpansion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DLExpansion
api_type:
- schema
ms.assetid: 9e50278d-fe6a-45e2-a72b-0fb06809e128
description: O elemento DLExpansion contém uma matriz de caixas de correio que estão contidos em uma lista de distribuição.
ms.openlocfilehash: 06081b4aba761a7137f921b3bc1c8d6b2afab88c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751909"
---
# <a name="dlexpansion"></a>DLExpansion

O elemento **DLExpansion** contém uma matriz de caixas de correio que estão contidos em uma lista de distribuição. 
  
- [ExpandDLResponse](expanddlresponse.md) 
- [ResponseMessages](responsemessages.md) 
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
- [DLExpansion](dlexpansion.md)
  
```xml
<DLExpansion AbsoluteDenominator"" IncludesLastItemInRange="" IndexedPagingOffset="" NumeratorOffset="" TotalItemsInView="">
   <Mailbox/>
</DLExpansion>
```

 **ArrayOfDLExpansionType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**IndexedPagingOffset** <br/> |Representa o próximo índice que deve ser usado para a próxima solicitação quando você estiver usando um modo de exibição de página indexados.  <br/> |
|**NumeratorOffset** <br/> |Representa o novo valor numerador a ser usado para a próxima solicitação quando você estiver usando os modos de exibição de página de fração.  <br/> |
|**AbsoluteDenominator** <br/> |Representa o denominador próximo a ser usado para a próxima solicitação quando você estiver usando os modos de exibição de página de fração.  <br/> |
|**IncludesLastItemInRange** <br/> |Indica se os resultados atuais contêm o último item na consulta de forma que não é necessária a paginação adicional.  <br/> |
|**TotalItemsInView** <br/> |Representa o número total de itens no modo de exibição.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Caixa de correio](mailbox.md) <br/> |Identifica um objeto de serviço de diretório do Active Directory habilitado para email.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação ExpandDL.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação ExpandDL](expanddl-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md) 
- [Referência do EWS para Exchange](ews-reference-for-exchange.md)

