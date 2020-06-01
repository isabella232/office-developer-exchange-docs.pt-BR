---
title: DelegateUser
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegateUser
api_type:
- schema
ms.assetid: aac4e74e-f69b-4c41-a0c9-489610330fbf
description: O elemento DelegateUser identifica um único representante para adicionar ou atualizar em uma caixa de correio ou um Representante retornado em uma resposta de gerenciamento de representante. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 40d9dacbd544436a3edf3213cf078cd33f961a74
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458800"
---
# <a name="delegateuser"></a>DelegateUser

O elemento **DelegateUser** identifica um único representante para adicionar ou atualizar em uma caixa de correio ou um Representante retornado em uma resposta de gerenciamento de representante. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<DelegateUser>
   <UserId/>
   <DelegatePermissions/>
   <ReceiveCopiesOfMeetingMessages/>
   <ViewPrivateItems/>
</DelegateUser>
```

**DelegateUserType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UserId](userid.md) <br/> |Identifica o representante. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[DelegatePermissions](delegatepermissions.md) <br/> |Contém as configurações de nível de permissão de representante. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[ReceiveCopiesOfMeetingMessages](receivecopiesofmeetingmessages.md) <br/> |Indica se um representante recebe cópias de mensagens relacionadas à reunião endereçadas à entidade de segurança. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[ViewPrivateItems](viewprivateitems.md) <br/> |Indica se um representante tem permissão para exibir itens de calendário privados na caixa de correio da entidade de segurança. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DelegateUsers](delegateusers.md) <br/> |Contém as identidades dos representantes a serem adicionadas ou atualizadas em uma caixa de correio.  <br/> |
|[DelegateUserResponseMessageType](delegateuserresponsemessagetype.md) <br/> |Contém mensagens de resposta para operações de gerenciamento de representante. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação AddDelegate](adddelegate-operation.md) 
- [Operação UpdateDelegate](updatedelegate-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Adicionar representantes](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

