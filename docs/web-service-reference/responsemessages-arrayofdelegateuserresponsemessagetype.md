---
title: ResponseMessages (ArrayOfDelegateUserResponseMessageType)
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
ms.assetid: 14819975-ce54-4f0e-9f90-d4b275895ea0
description: O elemento ResponseMessages contém as mensagens de resposta para uma solicitação de gerenciamento do representante de serviços Web do Exchange.
ms.openlocfilehash: e4b5567f3ded003e9648eb8ebebfadf8f1748d6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825193"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a>ResponseMessages (ArrayOfDelegateUserResponseMessageType)

O elemento **ResponseMessages** contém as mensagens de resposta para uma solicitação de gerenciamento do representante de serviços Web do Exchange. 
  
```
<ResponseMessages>
   <DelegateUserResponseMessageType/>
</ResponseMessages>
```

 **ArrayOfDelegateUserResponseMessageType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DelegateUserResponseMessageType](delegateuserresponsemessagetype.md) <br/> |Contém mensagens de resposta para operações de gerenciamento de representante.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Contém o status e o resultado de uma solicitação de [operação AddDelegate](adddelegate-operation.md) .  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Contém o status e o resultado de uma solicitação de [operação GetDelegate](getdelegate-operation.md) .  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |Contém o status e o resultado de uma solicitação de [operação UpdateDelegate](updatedelegate-operation.md) .  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |Contém o status e o resultado de uma solicitação de [operação RemoveDelegate](removedelegate-operation.md) .  <br/> |
   
## <a name="remarks"></a>Comentários

Esse elemento é usado a [operação AddDelegate](adddelegate-operation.md), a [operação de GetDelegate](getdelegate-operation.md), a [operação UpdateDelegate](updatedelegate-operation.md)e a [operação RemoveDelegate](removedelegate-operation.md). As respostas de operação de gerenciamento de representante são estruturadas de forma diferente de outras respostas. As mensagens de resposta do representante gerenciamento são fortemente tipadas.
  
O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server com a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação AddDelegate](adddelegate-operation.md)
  
[Operação GetDelegate](getdelegate-operation.md)
  
[Operação UpdateDelegate](updatedelegate-operation.md)
  
[Operação RemoveDelegate](removedelegate-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

