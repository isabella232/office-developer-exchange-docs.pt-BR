---
title: ApplyConversationActionResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ApplyConversationActionResponseMessage
api_type:
- schema
ms.assetid: a09edc89-7f2f-4846-a3a5-06694c97b9f6
description: O elemento ApplyConversationActionResponseMessage contém o status e os resultados de uma solicitação de operação ApplyConversationAction.
ms.openlocfilehash: 81378c822a473d969035f46f34ffca8939d7059d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522044"
---
# <a name="applyconversationactionresponsemessage"></a>ApplyConversationActionResponseMessage

O **elemento ApplyConversationActionResponseMessage** contém o status e os resultados de uma solicitação de operação [ApplyConversationAction.](applyconversationaction-operation.md)  
  
- [ApplyConversationActionResponse](applyconversationactionresponse.md)
- [ResponseMessages](responsemessages.md)
- [ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md)
  
```XML
<ApplyConversationActionResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ApplyConversationActionResponseMessage>
```

 **ApplyConversationActionResponseMessageType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**ResponseClass** <br/> | Descreve o status da resposta.<br/><br/>Os seguintes valores são válidos para este atributo:<ul><li>Sucesso</li><li>Aviso</li><li>Erro</li></ul> |
   
#### <a name="responseclass-attribute-values"></a>Valores de atributo ResponseClass

|**Valor**|**Descrição**|
|:-----|:-----|
|**Success** <br/> |Descreve uma solicitação que é atendida.  <br/> |
|**Aviso** <br/> | Descreve uma solicitação que não foi processada. Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e os itens subsequentes não puderam ser processados.<br/><br/>Veja a seguir exemplos de fontes de avisos:<ul><li>O Exchange store está offline durante o lote.</li><li>Os Serviços de Domínio do Active Directory (AD DS) estão offline.</li><li>Caixas de correio foram movidas.</li><li>O banco de dados de mensagens (MDB) está offline.</li><li>Uma senha expirou.</li><li>Uma cota foi excedida.</li></ul> |
|**Erro** <br/> | Descreve uma solicitação que não pode ser atendida.<br/><br/>Veja a seguir exemplos de fontes de erros:  <ul><li>Atributos ou elementos inválidos</li><li>Atributos ou elementos que estão fora do intervalo</li><li>Uma marca desconhecida  </li><li>Um atributo ou elemento que não é válido no contexto</li><li>Uma tentativa de acesso não autorizada por qualquer cliente</li><li>Uma falha no lado do servidor em resposta a uma chamada válida do lado do cliente</li></ul>Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText.](messagetext.md)  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fornece um código de erro que identifica o erro específico encontrado pela solicitação.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Atualmente não usado e reservado para uso futuro. Esse elemento contém um valor 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fornece informações adicionais de resposta a erros.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contém as mensagens de resposta para uma solicitação Exchange Web Services.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services. Esse elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
### <a name="version-differences"></a>Diferenças de versão

Em versões do Exchange a partir da com build 15.00.0986.00, o **elemento ApplyConversationActionResponseMessage** é do tipo **ApplyConversationActionResponseMessageType**. Nas versões anteriores, o elemento é do tipo **ResponseMessageType**.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação ApplyConversationAction](applyconversationaction-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

