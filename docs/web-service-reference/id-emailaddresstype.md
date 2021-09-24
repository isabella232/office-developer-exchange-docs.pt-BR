---
title: Id (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Id
api_type:
- schema
ms.assetid: 3e1e37b5-5469-4447-ad1f-c2c6d4e0482f
description: O elemento Id identifica uma sala de reunião dentro da organização Exchange servidor.
ms.openlocfilehash: 40f2163c4525e766e0fe0377820e87a806562001
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525819"
---
# <a name="id-emailaddresstype"></a>Id (EmailAddressType)

O **elemento Id** identifica uma sala de reunião dentro da organização Exchange servidor. 
  
[Room](room.md)
  
[Id (EmailAddressType)](id-emailaddresstype.md)
  
```xml
<Id>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Id>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Name (EmailAddressType)](name-emailaddresstype.md) <br/> |Define o nome da sala de reunião. Esse elemento é opcional.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Define o endereço SMTP (Simple Mail Transfer Protocol) de uma sala de reunião. Esse elemento é opcional.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Define o roteamento usado para a caixa de correio. O padrão é SMTP. Esse elemento é opcional.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Define o tipo de caixa de correio de um usuário de caixa de correio. Esse elemento é opcional.  <br/> |
|[ItemId](itemid.md) <br/> |Define o identificador de item de um contato ou lista de distribuição privada para destinatários da pasta de contatos de um usuário. Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Room](room.md) <br/> |Define uma sala de reunião na organização Exchange servidor.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório EWS do computador que está executando Microsoft Exchange Server que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetRooms](getrooms-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

