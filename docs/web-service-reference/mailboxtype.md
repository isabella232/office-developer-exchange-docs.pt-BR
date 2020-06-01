---
title: MailboxType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxType
api_type:
- schema
ms.assetid: 696e5fdb-d8c5-40f0-9e79-885eae65dfa4
description: O elemento MailboxType representa o tipo de caixa de correio que é representado pelo endereço de email.
ms.openlocfilehash: 8c322ab8a87730832f5d199698a369656b058a9a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459795"
---
# <a name="mailboxtype"></a>MailboxType

O elemento **MailboxType** representa o tipo de caixa de correio que é representado pelo endereço de email. 
  
```XML
<MailboxType>Mailbox | PublicDL | PrivateDL | Contact | PublicFolder | Unknown | OneOff | GroupMailbox</MailboxType>
```

**MailboxTypeType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Caixa de Correio](mailbox.md) <br/> |Identifica um endereço de email totalmente resolvido.  <br/> |
|[RoomList](roomlist.md) <br/> |Identifica uma lista de salas de reunião.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o elemento **MailboxType** . 
  
|**Valor**|**Descrição**|
|:-----|:-----|
|Caixa de correio  <br/> |Representa um objeto do Active Directory habilitado para email.  <br/> |
|PublicDL  <br/> |Representa uma lista de distribuição pública.  <br/> |
|PrivateDL  <br/> |Representa uma lista de distribuição privada na caixa de correio de um usuário.  <br/> |
|Contato  <br/> |Representa um contato na caixa de correio de um usuário.  <br/> |
|PublicFolder  <br/> |Representa uma pasta pública.  <br/> |
|Desconhecido  <br/> |Representa um tipo desconhecido de caixa de correio.  <br/> |
|OneOff  <br/> |Representa um membro one-off de uma lista de distribuição pessoal.  <br/> |
|GroupMailbox  <br/> |Representa uma caixa de correio de grupo.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

