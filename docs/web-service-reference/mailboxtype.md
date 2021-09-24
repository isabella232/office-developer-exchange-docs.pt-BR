---
title: MailboxType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailboxType
api_type:
- schema
ms.assetid: 696e5fdb-d8c5-40f0-9e79-885eae65dfa4
description: O elemento MailboxType representa o tipo de caixa de correio representada pelo endereço de email.
ms.openlocfilehash: f7605bf0e90851352efaaabed09e878be0925581
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524046"
---
# <a name="mailboxtype"></a>MailboxType

O **elemento MailboxType** representa o tipo de caixa de correio representada pelo endereço de email. 
  
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

A tabela a seguir lista os valores possíveis para o **elemento MailboxType.** 
  
|**Valor**|**Descrição**|
|:-----|:-----|
|Mailbox  <br/> |Representa um objeto Active Directory habilitado para email.  <br/> |
|PublicDL  <br/> |Representa uma lista de distribuição pública.  <br/> |
|PrivateDL  <br/> |Representa uma lista de distribuição privada na caixa de correio de um usuário.  <br/> |
|Contact  <br/> |Representa um contato na caixa de correio de um usuário.  <br/> |
|PublicFolder  <br/> |Representa uma pasta pública.  <br/> |
|Desconhecido  <br/> |Representa um tipo desconhecido de caixa de correio.  <br/> |
|OneOff  <br/> |Representa um membro único de uma lista de distribuição pessoal.  <br/> |
|GroupMailbox  <br/> |Representa uma caixa de correio de grupo.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

