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
description: O elemento DLExpansion contém uma matriz de caixas de correio que estão contidas em uma lista de distribuição.
ms.openlocfilehash: 079ad1c0f114d201f5d1b91c3fd9bb45b943cc1a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456994"
---
# <a name="dlexpansion"></a>DLExpansion

O elemento **DLExpansion** contém uma matriz de caixas de correio que estão contidas em uma lista de distribuição. 
  
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
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**IndexedPagingOffset** <br/> |Representa o próximo índice que deve ser usado para a próxima solicitação quando você estiver usando um modo de exibição de página indexado.  <br/> |
|**NumeratorOffset** <br/> |Representa o novo valor do numerador a ser usado para a próxima solicitação quando você estiver usando modos de exibição de página de fração.  <br/> |
|**AbsoluteDenominator** <br/> |Representa o próximo denominador a ser usado para a próxima solicitação quando você estiver usando modos de exibição de página de fração.  <br/> |
|**IncludesLastItemInRange** <br/> |Indica se os resultados atuais contêm o último item na consulta para que a paginação adicional não seja necessária.  <br/> |
|**TotalItemsInView** <br/> |Representa o número total de itens no modo de exibição.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Caixa de Correio](mailbox.md) <br/> |Identifica um objeto de serviço de diretório do Active Directory habilitado para email.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de ExpandDL.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação ExpandDL](expanddl-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md) 
- [Referência do EWS para Exchange](ews-reference-for-exchange.md)

