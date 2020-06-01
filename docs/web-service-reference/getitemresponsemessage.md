---
title: GetItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItemResponseMessage
api_type:
- schema
ms.assetid: cc583723-54d1-4a17-8c1f-6586f70fdefd
description: O elemento GetItemResponseMessage contém o status e o resultado de uma única solicitação de operação de GetItem.
ms.openlocfilehash: bd25a82641259e1546bad6eef5c2f6f8f03e98cb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458667"
---
# <a name="getitemresponsemessage"></a>GetItemResponseMessage

O elemento **GetItemResponseMessage** contém o status e o resultado de uma única solicitação de [operação de GetItem](getitem-operation.md) . 
  
- [GetItemResponse](getitemresponse.md) 
- [ResponseMessages](responsemessages.md)
- [GetItemResponseMessage](getitemresponsemessage.md)
  
```xml
<GetItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</GetItemResponseMessage>
```

**ItemInfoResponseMessageType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**ResponseClass** <br/> | Descreve o status de uma resposta de [operação do GetItem](getitem-operation.md) . <br/><br/>Os seguintes valores são válidos para este atributo:<br/><br/>-Êxito<br/>-Aviso<br/>-Erro |
   
#### <a name="responseclass-attribute-values"></a>Valores de atributo ResponseClass

|**Valor**|**Descrição**|
|:-----|:-----|
|**Success** <br/> |Descreve uma solicitação que é atendida.  <br/> |
|**Aviso** <br/> | Descreve uma solicitação que não foi processada. Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação foi processado e itens subsequentes não puderam ser processados.<br/><br/>Estes são exemplos de fontes para avisos:<br/><br/>– O repositório do Exchange está offline durante o lote.<br/>– Os serviços de domínio do Active Directory (AD DS) estão offline.<br/>-As caixas de correio são movidas.<br/>-O MDB está offline.<br/>-A senha expirou.  <br/>-A cota é excedida. |
|**Error** <br/> | Descreve uma solicitação que não pode ser atendida.<br/><br/>A seguir estão exemplos de fontes de erros:<br/><br/>-Atributos ou elementos inválidos<br/>-Atributos ou elementos fora do intervalo<br/>– Marca desconhecida<br/>-Atributo ou elemento não válido no contexto<br/>– Acesso não autorizado tentado por qualquer cliente<br/>-Falha do servidor em resposta a uma chamada válida do lado do cliente<br/><br/>As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) . |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fornece um código de erro que identifica o erro específico que a solicitação encontrou.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Não utilizado no momento e está reservado para uso futuro. Ele contém um valor de 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fornece informações adicionais de resposta de erro.  <br/> |
|[Itens](items.md) <br/> |Contém uma matriz de itens retornados.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [GetItem](getitem.md)
- [Operação GetItem](getitem-operation.md)

