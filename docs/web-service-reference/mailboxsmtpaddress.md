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
description: O elemento MailboxSmtpAddress representa o endereço SMTP do usuário cujas regras de caixa de entrada devem ser recuperadas ou atualizada; ou cuja data de expiração de senha deve ser recuperado.
ms.openlocfilehash: 60b2c018f2a05e9630e92e28de1054a421b41e52
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824303"
---
# <a name="mailboxsmtpaddress"></a>MailboxSmtpAddress

O elemento **MailboxSmtpAddress** representa o endereço SMTP do usuário cujas regras de caixa de entrada devem ser recuperadas ou atualizada; ou cuja data de expiração de senha deve ser recuperado. 
  
```XML
<MailboxSmtpAddress/>
```

**cadeia de caracteres**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetInboxRules](getinboxrules.md) <br/> |Define uma solicitação para obter as regras de caixa de entrada em uma caixa de correio no armazenamento do servidor.  <br/> |
|[GetPasswordExpirationDate](getpasswordexpirationdate.md) <br/> |Define uma solicitação para obter a data de expiração de senha de uma conta de email.  <br/> |
|[UpdateInboxRules](updateinboxrules.md) <br/> |Define uma solicitação para atualizar as regras de caixa de entrada em uma caixa de correio no armazenamento do servidor.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O **MailboxSmtpAddress** é um elemento opcional. Se o elemento **MailboxSmtpAddress** for omitido, o endereço do usuário conectado é usado. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação GetInboxRules](getinboxrules-operation.md)
- [Operação GetPasswordExpirationDate](getpasswordexpirationdate-operation.md)
- [Operação UpdateInboxRules](updateinboxrules-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

