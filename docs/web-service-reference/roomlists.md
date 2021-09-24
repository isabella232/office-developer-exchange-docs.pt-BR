---
title: RoomLists
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RoomLists
api_type:
- schema
ms.assetid: 2b190823-b11e-4635-97e4-3aba5865fd05
description: O elemento RoomLists é uma lista de um ou mais endereços que representam uma lista de salas de reunião.
ms.openlocfilehash: e2825ccf5f660e00da61a605282613c07678a74b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523486"
---
# <a name="roomlists"></a>RoomLists

O **elemento RoomLists** é uma lista de um ou mais endereços que representam uma lista de salas de reunião. 
  
[GetRoomListsResponse](getroomlistsresponse.md)
  
[RoomLists](roomlists.md)
  
```xml
<RoomLists>   <Address/></RoomLists>
```

 **ArrayOfEmailAddressesType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Address (EmailAddressType)](address-emailaddresstype.md) <br/> |Define o endereço de email e o nome de exibição que representa a lista de sala. Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetRoomListsResponse](getroomlistsresponse.md) <br/> |Contém o status e o resultado de uma solicitação de operação [GetRoomLists.](getroomlists-operation.md)  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Exchange Server com a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetRoomLists](getroomlists-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

