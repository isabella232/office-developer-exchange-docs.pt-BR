---
title: GetStreamingEventsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEventsResponseMessage
api_type:
- schema
ms.assetid: 655e4e78-af74-48b0-a988-7d86ab368feb
description: O elemento GetStreamingEventsResponseMessage contém o status e o resultado de uma única solicitação de operação de GetStreamingEvents.
ms.openlocfilehash: 055fb7eeb12e241739eb860cecbe398b8a322bd2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459143"
---
# <a name="getstreamingeventsresponsemessage"></a>GetStreamingEventsResponseMessage

O elemento **GetStreamingEventsResponseMessage** contém o status e o resultado de uma única solicitação de [operação de GetStreamingEvents](getstreamingevents-operation.md) . 
  
```xml
<GetStreamingEventsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notifications/>
   <ErrorSubscriptionIds/>
   <ConnectionStatus/>
</GetStreamingEventsResponseMessage>
```

 **GetStreamingEventsResponseMessageType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**ResponseClass** <br/> | Descreve o status de uma resposta de [operação do GetStreamingEvents](getstreamingevents-operation.md) . <br/><br/>Os seguintes valores são válidos para este atributo:  <br/><br/>-Êxito  <br/>-Aviso  <br/>-Erro  <br/> |
   
#### <a name="responseclass-attribute"></a>Atributo ResponseClass

|**Valor**|**Descrição**|
|:-----|:-----|
|Êxito  <br/> |Descreve uma solicitação que é atendida.  <br/> |
|Aviso  <br/> | Descreve uma solicitação que não foi processada. Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes. <br/><br/>A seguir estão exemplos de fontes de avisos:  <br/><br/>– O repositório do Exchange está offline durante o lote.  <br/>– Os serviços de domínio do Active Directory (AD DS) estão offline.  <br/>-As caixas de correio foram movidas.  <br/>– O banco de dados de caixa de correio (MDB) está offline.  <br/>-Uma senha expirou.  <br/>-Uma cota foi excedida.  <br/> |
|Erro  <br/> | Descreve uma solicitação que não pode ser atendida. <br/><br/>A seguir estão exemplos de fontes de erros:  <br/><br/>-Atributos ou elementos inválidos  <br/>-Atributos ou elementos que estão fora do intervalo  <br/>-Uma marca desconhecida  <br/>-Um atributo ou elemento que não é válido no contexto  <br/>– Uma tentativa de acesso não autorizado por qualquer cliente  <br/>-Uma falha do servidor em resposta a uma chamada válida do lado do cliente  <br/><br/>  As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fornece um código de erro que identifica o erro específico que a solicitação encontrou.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Não utilizado no momento e está reservado para uso futuro. Ele contém um valor de 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fornece informações adicionais de resposta de erro.  <br/> |
|[Notificações](notifications.md) <br/> |Contém uma lista de informações sobre a assinatura e os eventos que ocorreram desde a última notificação.  <br/> |
|[ErrorSubscriptionIds](errorsubscriptionids.md) <br/> |Contém uma lista de IDs de assinatura que são inválidas.  <br/> |
|[ConnectionStatus](connectionstatus.md) <br/> |Fornece uma descrição de texto do status de uma assinatura de streaming.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [GetStreamingEvents](getstreamingevents.md) 
- [GetStreamingEventsResponse](getstreamingeventsresponse.md)
- [Operação GetStreamingEvents](getstreamingevents-operation.md)

