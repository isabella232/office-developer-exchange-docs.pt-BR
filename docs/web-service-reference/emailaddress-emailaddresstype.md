---
title: EmailAddress (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0cdabfcb-7658-4c7d-bb03-1e776ed11e43
description: O elemento EmailAddress especifica o endereço SMTP totalmente resolvido para a caixa de correio do site ou a persona associada.
ms.openlocfilehash: 76b279a82f6f277d9f231866437359ceae46df59
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545255"
---
# <a name="emailaddress-emailaddresstype"></a>EmailAddress (EmailAddressType)

O **elemento EmailAddress** especifica o endereço SMTP totalmente resolvido para a caixa de correio do site ou a persona associada. 
  
```xml
<EmailAddress>
    <Name></Name>
    <EmailAddress></EmailAddress>
    <RoutingType></RoutingType>
    <MailboxType></MailboxType>
    <ItemId></ItemId>
</EmailAddress>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Name (string)](name-string.md) <br/> |Especifica um nome ou chave do refinador de pesquisa ou o nome de um usuário de email.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Define o endereço SMTP principal de um usuário de caixa de correio.  <br/> |
|[RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) <br/> |Especifica o tipo de roteamento de um endereço de email.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Representa o tipo de caixa de correio representada pelo endereço de email.  <br/> |
|[ItemId](itemid.md) <br/> |Contém o identificador exclusivo e a chave de alteração de um item no Exchange store.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Pessoal](persona.md) <br/> |Especifica um conjunto de dados de persona retornados por uma **solicitação GetPersona.**  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

Esse elemento é opcional.
  
O **elemento EmailAddress** é aplicável para clientes destinados Exchange Online e versões do Microsoft Exchange Server a partir Exchange 2013. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Tipo de esquema  <br/> |
|Arquivo de validação  <br/> |types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

