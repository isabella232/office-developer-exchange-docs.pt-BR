---
title: SubscribeResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscribeResponseMessage
api_type:
- schema
ms.assetid: d121d38a-a61a-4f9c-a477-fc6d7f9af77e
description: O elemento SubscribeResponseMessage contém o status e o resultado de uma única solicitação de operação de assinatura.
ms.openlocfilehash: eea7356dbcf1887383d56e40a4f6dcd091535fa3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465370"
---
# <a name="subscriberesponsemessage"></a>SubscribeResponseMessage

O elemento **SubscribeResponseMessage** contém o status e o resultado de uma única solicitação de [operação de assinatura](subscribe-operation.md) . 
  
- [SubscribeResponse](subscriberesponse.md)
- [ResponseMessages](responsemessages.md)
- [SubscribeResponseMessage](subscriberesponsemessage.md)
  
```xml
<SubscribeResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SubscriptionId/>
   <Watermark/>
</SubscribeResponseMessage>
```

 **SubscribeResponseMessageType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**ResponseClass** <br/> | Descreve o status de uma resposta de [operação de assinatura](subscribe-operation.md) . <br/><br/>Os seguintes valores são válidos para este atributo:  <br/><br/>-Êxito  <br/>-Aviso  <br/>-Erro  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Valores de atributo ResponseClass

|**Valor**|**Descrição**|
|:-----|:-----|
|**Success** <br/> |Descreve uma solicitação que é atendida.  <br/> |
|**Aviso** <br/> | Descreve uma solicitação que não foi processada. Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes. <br/><br/>A seguir estão exemplos de fontes de avisos:  <br/><br/>– O repositório do Exchange está offline durante o lote.  <br/>– Os serviços de domínio do Active Directory (AD DS) estão offline.  <br/>-As caixas de correio foram movidas.  <br/>– O banco de dados de mensagens (MDB) está offline.  <br/>-Uma senha expirou.  <br/>-Uma cota foi excedida.  <br/> |
|**Error** <br/> | Descreve uma solicitação que não pode ser atendida. <br/><br/>A seguir estão exemplos de fontes de erros:  <br/><br/>-Atributos ou elementos inválidos  <br/>-Atributos ou elementos que estão fora do intervalo  <br/>-Uma marca desconhecida  <br/>-Um atributo ou elemento que não é válido no contexto  <br/>– Uma tentativa de acesso não autorizado por qualquer cliente  <br/>-Uma falha do servidor em resposta a uma chamada válida do lado do cliente  <br/><br/>  As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fornece um código de erro que identifica o erro específico que a solicitação encontrou.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Atualmente não usado e reservado para uso futuro. Este elemento contém um valor de 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fornece informações adicionais de resposta de erro.  <br/> |
|[SubscriptionId (GetEvents)](subscriptionid-getevents.md) <br/> |Representa o identificador de uma assinatura.  <br/> |
|[Marca d'água](watermark.md) <br/> |Representa um indicador de evento na fila de eventos de caixa de correio.  <br/> |
   
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

- [Operação Subscribe](subscribe-operation.md)
- [Operação GetEvents](getevents-operation.md)
- [Cancelar a operação](unsubscribe-operation.md)

