---
title: ResponseMessages (ArrayOfMailTipsResponseMessageType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 00878187-fac2-45b9-ba1c-df7ffac71089
description: O elemento ResponseMessages representa uma lista das mensagens de resposta de dicas de email.
ms.openlocfilehash: 80610af191f3fa600abe2ba8dbba2aac63f3ab1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825192"
---
# <a name="responsemessages-arrayofmailtipsresponsemessagetype"></a>ResponseMessages (ArrayOfMailTipsResponseMessageType)

O elemento **ResponseMessages** representa uma lista das mensagens de resposta de dicas de email. 
  
```XML
<ResponseMessages>
   <MailTipsResponseMessageType/>
</ResponseMessages>
```

 **ArrayOfMailTipsResponseMessageType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MailTipsResponseMessageType](mailtipsresponsemessagetype.md) <br/> |Representa as configurações de dicas de email.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetMailTipsResponse](getmailtipsresponse.md) <br/> |Representa a mensagem de resposta para a [operação GetMailTips](getmailtips-operation.md).  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação GetMailTips](getmailtips-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

