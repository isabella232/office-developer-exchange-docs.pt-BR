---
title: ExpandDLResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExpandDLResponseMessage
api_type:
- schema
ms.assetid: 1140601b-98cf-4cb4-a019-321c7f63d5be
description: O elemento ExpandDLResponseMessage contém o status e o resultado de uma única solicitação de operação ExpandDL.
ms.openlocfilehash: 4683195af3daa462758acbfac4903994818a120e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517067"
---
# <a name="expanddlresponsemessage"></a>ExpandDLResponseMessage

O **elemento ExpandDLResponseMessage** contém o status e o resultado de uma única [solicitação de operação ExpandDL.](expanddl-operation.md) 
  
- [ExpandDLResponse](expanddlresponse.md)  
- [ResponseMessages](responsemessages.md) 
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
  
```xml
<ExpandDLResponseMessage ResponseClass="" IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DLExpansion/>
</ExpandDLResponseMessage>
```

**ExpandDLResponseMessageType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**ResponseClass** <br/> | Descreve o status de uma resposta [de operação ExpandDL.](expanddl-operation.md)<br/><br/>Os seguintes valores são válidos para este atributo: <br/> <br/>- Sucesso  <br/>- Aviso  <br/>- Erro  <br/> |
|**IndexedPagingOffset** <br/> |Representa o próximo índice que deve ser usado para a próxima solicitação quando um exibição de pajamento indexado é usado.  <br/> |
|**NumeratorOffset** <br/> |Representa o novo valor de numerador a ser usado para a próxima solicitação quando exibições de página de fração são usadas.  <br/> |
|**AbsoluteDenominator** <br/> |Representa o próximo denominador a ser usado para a próxima solicitação ao fazer pajamento fracional.  <br/> |
|**IncludesLastItemInRange** <br/> |Indica que a paja adicional não é necessária. Esse atributo será true se os resultados atuais conterem o último item na consulta.  <br/> |
|**TotalItemsInView** <br/> |Representa o número total de itens que passam na restrição.  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Valores de atributo ResponseClass

|**Valor**|**Descrição**|
|:-----|:-----|
|**Success** <br/> |Descreve uma solicitação que é atendida.  <br/> |
|**Aviso** <br/> | Descreve uma solicitação que não foi processada. Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e os itens subsequentes não puderam ser processados.<br/><br/> Veja a seguir exemplos de fontes de avisos:<br/>  <br/>- O Exchange store está offline durante o lote.  <br/>- Os Serviços de Domínio do Active Directory (AD DS) estão offline.  <br/>- As caixas de correio são movidas.  <br/>- O banco de dados de caixa de correio (MDB) está offline.  <br/>- Uma senha expirou.  <br/>- Uma cota foi excedida.  <br/> |
|**Erro** <br/> | Descreve uma solicitação que não pode ser atendida.<br/><br/> Veja a seguir exemplos de fontes de erros:  <br/><br/>- Atributos ou elementos inválidos  <br/>- Atributos ou elementos que estão fora do intervalo  <br/>- Uma marca desconhecida  <br/>- Um atributo ou elemento que não é válido no contexto  <br/>- Uma tentativa de acesso não autorizada por qualquer cliente  <br/>- Uma falha no lado do servidor em resposta a uma chamada válida do lado do cliente <br/> <br/>  Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText.](messagetext.md)  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fornece um código de erro que identifica o erro específico encontrado pela solicitação.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Atualmente não usado e reservado para uso futuro. Ele contém um valor 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fornece informações adicionais de resposta a erros.  <br/> |
|[DLExpansion](dlexpansion.md) <br/> |Contém uma matriz de caixas de correio que estão contidas em uma lista de distribuição.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contém as mensagens de resposta para uma solicitação Exchange Web Services.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Exchange Server com a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação ExpandDL](expanddl-operation.md)
- [Referência do EWS para Exchange](ews-reference-for-exchange.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

