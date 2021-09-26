---
title: MailboxFull
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailboxFull
api_type:
- schema
ms.assetid: 38b28c9b-9da2-4d6a-9cda-9c393986575b
description: O elemento MailboxFull indica se a caixa de correio do destinatário está cheia.
ms.openlocfilehash: 919f05a69f1436dbc37e27f12e32b5099bd09028
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544854"
---
# <a name="mailboxfull"></a>MailboxFull

O **elemento MailboxFull** indica se a caixa de correio do destinatário está cheia. 
  
```XML
<MailboxFull>true | false</MailboxFull>
```

**Boolean**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Dicas de Email](mailtips.md) <br/> |Representa valores para vários tipos de dicas de email.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Esse elemento pode ser **verdadeiro ou** **falso.** Um valor **verdadeiro** indica que a caixa de correio atingiu sua capacidade; um valor **false** indica que ele não atingiu a capacidade. 
  
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

