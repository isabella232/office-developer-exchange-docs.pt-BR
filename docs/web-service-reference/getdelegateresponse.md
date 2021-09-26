---
title: GetDelegateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetDelegateResponse
api_type:
- schema
ms.assetid: 71a418a5-5652-40e1-8f84-fe4f7c9f86af
description: O elemento GetDelegateResponse contém o status e o resultado de uma solicitação de operação GetDelegate.
ms.openlocfilehash: d8550ede774ebe0e84cb2da27455465c330fbf3c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546319"
---
# <a name="getdelegateresponse"></a>GetDelegateResponse

O **elemento GetDelegateResponse** contém o status e o resultado de uma solicitação de operação [GetDelegate.](getdelegate-operation.md) 
  
```xml
<GetDelegateResponse>
   <DeliverMeetingRequests/>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</GetDelegateResponse>
```

 **GetDelegateResponseMessageType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DeliverMeetingRequests](delivermeetingrequests.md) <br/> |Define como as solicitações de reunião são tratadas entre o representante e a entidade principal.  <br/> |
|[ResponseMessages (ArrayOfDelegateUserResponseMessageType)](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |Contém as mensagens de resposta para uma solicitação Exchange de gerenciamento de representantes dos Serviços Web.  <br/> |
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fornece um código de erro que identifica o erro específico encontrado pela solicitação.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Atualmente não usado e reservado para uso futuro. Ele contém um valor 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fornece informações adicionais de resposta a erros.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2010 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetDelegate](getdelegate-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

