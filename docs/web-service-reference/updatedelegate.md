---
title: UpdateDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateDelegate
api_type:
- schema
ms.assetid: c6ae99c4-18b0-4136-90ab-12cf15e15f91
description: O elemento UpdateDelegate define uma solicitação para atualizar representantes em uma caixa de correio. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: e4e5f79a54e6555a8758612fa02d897df5c3f0af
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541802"
---
# <a name="updatedelegate"></a>UpdateDelegate

O **elemento UpdateDelegate** define uma solicitação para atualizar representantes em uma caixa de correio. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<UpdateDelegate>
      <DelegateUsers/>
   <DeliverMeetingRequests/>
      <Mailbox/>
</UpdateDelegate>
```

 **UpdateDelegateType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DelegateUsers](delegateusers.md) <br/> |Contém uma matriz [de elementos DelegateUser](delegateuser.md) que identificam os representantes e as atualizações a aplicar aos representantes. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[DeliverMeetingRequests](delivermeetingrequests.md) <br/> |Define como as solicitações de reunião são tratadas entre o representante e a entidade principal. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[Caixa de Correio](mailbox.md) <br/> |Identifica um objeto de serviço de diretório do Active Directory habilitado para email.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação UpdateDelegate](updatedelegate-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

