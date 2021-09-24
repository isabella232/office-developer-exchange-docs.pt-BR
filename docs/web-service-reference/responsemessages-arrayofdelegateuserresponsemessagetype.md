---
title: ResponseMessages (ArrayOfDelegateUserResponseMessageType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 14819975-ce54-4f0e-9f90-d4b275895ea0
description: O elemento ResponseMessages contém as mensagens de resposta para uma solicitação de gerenciamento de representantes Exchange Web Services.
ms.openlocfilehash: aa90d2572679ecf3e5d99cc55731d388e083ff01
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525564"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a>ResponseMessages (ArrayOfDelegateUserResponseMessageType)

O **elemento ResponseMessages** contém as mensagens de resposta para uma solicitação Exchange de gerenciamento de representantes dos Serviços Web. 
  
```
<ResponseMessages>
   <DelegateUserResponseMessageType/>
</ResponseMessages>
```

 **ArrayOfDelegateUserResponseMessageType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DelegateUserResponseMessageType](delegateuserresponsemessagetype.md) <br/> |Contém mensagens de resposta para operações de gerenciamento de representantes.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Contém o status e o resultado de uma [solicitação de operação AddDelegate.](adddelegate-operation.md)  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Contém o status e o resultado de uma [solicitação de operação GetDelegate.](getdelegate-operation.md)  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |Contém o status e o resultado de uma [solicitação de operação UpdateDelegate.](updatedelegate-operation.md)  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |Contém o status e o resultado de uma [solicitação de operação RemoveDelegate.](removedelegate-operation.md)  <br/> |
   
## <a name="remarks"></a>Comentários

Esse elemento é usado na operação [AddDelegate,](adddelegate-operation.md)na operação [GetDelegate,](getdelegate-operation.md)na [operação UpdateDelegate](updatedelegate-operation.md)e na [operação RemoveDelegate.](removedelegate-operation.md) As respostas da operação de gerenciamento de representantes são estruturadas de forma diferente de outras respostas. As mensagens de resposta de gerenciamento de representantes são fortemente digitadas.
  
O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Exchange Server com a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação AddDelegate](adddelegate-operation.md)
  
[Operação GetDelegate](getdelegate-operation.md)
  
[Operação UpdateDelegate](updatedelegate-operation.md)
  
[Operação RemoveDelegate](removedelegate-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

