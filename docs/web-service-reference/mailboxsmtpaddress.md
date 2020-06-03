---
title: MailboxSmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxSmtpAddress
api_type:
- schema
ms.assetid: de7c9035-ebbc-4473-ac14-3b22ce62768c
description: O elemento MailboxSmtpAddress representa o endereço SMTP do usuário cujas regras de caixa de entrada devem ser recuperadas ou atualizadas; ou cuja data de expiração de senha deve ser recuperada.
ms.openlocfilehash: 613e8098210257280bec47f2b22a2d29d04fa07c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530541"
---
# <a name="mailboxsmtpaddress"></a>MailboxSmtpAddress

O elemento **MailboxSmtpAddress** representa o endereço SMTP do usuário cujas regras de caixa de entrada devem ser recuperadas ou atualizadas; ou cuja data de expiração de senha deve ser recuperada. 
  
```XML
<MailboxSmtpAddress/>
```

**cadeia de caracteres**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetInboxRules](getinboxrules.md) <br/> |Define uma solicitação para obter as regras de caixa de entrada em uma caixa de correio no repositório do servidor.  <br/> |
|[GetPasswordExpirationDate](getpasswordexpirationdate.md) <br/> |Define uma solicitação para obter a data de expiração da senha de uma conta de email.  <br/> |
|[UpdateInboxRules](updateinboxrules.md) <br/> |Define uma solicitação para atualizar as regras de caixa de entrada em uma caixa de correio no repositório do servidor.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O elemento **MailboxSmtpAddress** é um elemento opcional. Se o elemento **MailboxSmtpAddress** for omitido, o endereço do usuário conectado será usado. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetInboxRules](getinboxrules-operation.md)
- [Operação GetPasswordExpirationDate](getpasswordexpirationdate-operation.md)
- [Operação UpdateInboxRules](updateinboxrules-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

