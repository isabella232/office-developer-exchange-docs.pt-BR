---
title: EmailAddress (EmailAddresstype)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cdabfcb-7658-4c7d-bb03-1e776ed11e43
description: O elemento EmailAddress especifica o endereço SMTP totalmente resolvido para a caixa de correio do site ou a pessoa associada.
ms.openlocfilehash: 8b04b75e91cc16be7f88c9a0ac08c5e36855056e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463458"
---
# <a name="emailaddress-emailaddresstype"></a>EmailAddress (EmailAddresstype)

O elemento **EmailAddress** especifica o endereço SMTP totalmente resolvido para a caixa de correio do site ou a pessoa associada. 
  
```xml
<EmailAddress>
    <Name></Name>
    <EmailAddress></EmailAddress>
    <RoutingType></RoutingType>
    <MailboxType></MailboxType>
    <ItemId></ItemId>
</EmailAddress>
```

 **EmailAddresstype**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Nome (cadeia de caracteres)](name-string.md) <br/> |Especifica um nome ou chave de refinador de pesquisa ou o nome de um usuário de email.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Define o endereço SMTP principal de um usuário de caixa de correio.  <br/> |
|[RoutingType (EmailAddresstype)](routingtype-emailaddresstype.md) <br/> |Especifica o tipo de roteamento de um endereço de email.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Representa o tipo de caixa de correio que é representado pelo endereço de email.  <br/> |
|[ItemId](itemid.md) <br/> |Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Pessoal](persona.md) <br/> |Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

Este elemento é opcional.
  
O elemento **EmailAddress** é aplicável para clientes que direcionam o Exchange Online e versões do Microsoft Exchange Server a partir do Exchange 2013. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Também consulte

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

