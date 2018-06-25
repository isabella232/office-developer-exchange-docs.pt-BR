---
title: EmailAddress (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cdabfcb-7658-4c7d-bb03-1e776ed11e43
description: O elemento EmailAddress Especifica o endereço SMTP completamente resolvido para a caixa de correio de site ou a pessoa associada.
ms.openlocfilehash: c31a37fc0dbdcc2b501b82346a17a0a3b4775556
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751984"
---
# <a name="emailaddress-emailaddresstype"></a>EmailAddress (EmailAddressType)

O elemento **EmailAddress** Especifica o endereço SMTP completamente resolvido para a caixa de correio de site ou a pessoa associada. 
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Nome (string)](name-string.md) <br/> |Especifica o nome de um usuário de email ou um nome de refinador de pesquisa ou chave.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Define o endereço SMTP principal de um usuário de caixa de correio.  <br/> |
|[RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) <br/> |Especifica o tipo de roteamento de um endereço de email.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Representa o tipo de caixa de correio que é representado por um endereço de email.  <br/> |
|[ItemId](itemid.md) <br/> |Contém o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Pessoa](persona.md) <br/> |Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

Esse elemento é opcional.
  
O elemento **EmailAddress** é aplicável para clientes que visam o Exchange Online e versões do Microsoft Exchange Server, começando com o Exchange 2013. 
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

