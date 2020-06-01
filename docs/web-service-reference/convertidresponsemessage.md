---
title: ConvertIdResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertIdResponseMessage
api_type:
- schema
ms.assetid: 7a439cae-0268-4328-9ded-af56ad642227
description: O elemento ConvertIdResponseMessage contém o status e o resultado de uma solicitação de operação convertid.
ms.openlocfilehash: cd0154f87390be3516ced4be53f5371d4a348c49
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456217"
---
# <a name="convertidresponsemessage"></a>ConvertIdResponseMessage

O elemento **ConvertIdResponseMessage** contém o status e o resultado de uma solicitação de [operação convertid](convertid-operation.md) . 
  
- [ConvertIdResponse](convertidresponse.md) 
- [ResponseMessages](responsemessages.md)
- [ConvertIdResponseMessage](convertidresponsemessage.md)
  
```xml
<ConvertIdResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <AlternateId/>
</ConvertIdResponseMessage>
```

 **ConvertIdResponseMessageType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**ResponseClass** <br/> | Descreve o status de uma resposta de [operação convertid](convertid-operation.md) .<br/><br/>Os seguintes valores são válidos para este atributo:<br/><br/>-Êxito  <br/>-Aviso  <br/>-Erro  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Valores de atributo ResponseClass

|**Valor**|**Descrição**|
|:-----|:-----|
|**Success** <br/> |Descreve uma solicitação que é atendida.  <br/> |
|**Aviso** <br/> | Descreve uma solicitação que não foi totalmente processada ou para a qual ocorreu um resultado não desejado.  <br/> |
|**Error** <br/> | Descreve uma solicitação que não pode ser atendida.<br/><br/>A seguir estão exemplos de fontes de erros:  <br/><br/>-Atributos ou elementos inválidos  <br/>-Atributos ou elementos que estão fora do intervalo  <br/>-Uma marca desconhecida  <br/>-Um atributo ou elemento que não é válido no contexto  <br/>– Uma tentativa de acesso não autorizado por qualquer cliente  <br/>-Uma falha do servidor em resposta a uma chamada válida do lado do cliente<br/><br/>As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fornece um código de erro que identifica o erro específico que a solicitação encontrou.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Atualmente não usado e reservado para uso futuro. Este elemento contém um valor de 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fornece informações adicionais de resposta de erro.  <br/> |
|[AlternateId](alternateid.md) <br/> |Descreve um identificador convertido na resposta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.  <br/> |
   
## <a name="remarks"></a>Comentários

Uma mensagem de resposta por identificador convertido é retornada. O elemento [alternateid](alternateid.md) estará ausente da resposta se um código de resposta de erro for retornado. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Exchange 2010 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação convertid](convertid-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

