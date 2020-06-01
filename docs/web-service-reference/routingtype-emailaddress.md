---
title: RoutingType (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoutingType
api_type:
- schema
ms.assetid: 74d83198-0d9d-4c78-a2bc-9a671859ff37
description: O elemento RoutingType representa o protocolo de roteamento para o destinatário.
ms.openlocfilehash: 2193e72c38c687669f6e052b4d2526029aa89d89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459031"
---
# <a name="routingtype-emailaddress"></a>RoutingType (EmailAddress)

O elemento **RoutingType** representa o protocolo de roteamento para o destinatário. 
  
```XML
<RoutingType/>
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
|[Email (EmailAddresstype)](email-emailaddresstype.md) <br/> |Especifica o endereço de email do objeto MailboxData. Este elemento é usado na [operação GetUserAvailability](getuseravailability-operation.md).  <br/><br/> Este é o XPath para este elemento:  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[Caixa de correio (disponibilidade)](mailbox-availability.md) <br/> | Representa o usuário de caixa de correio de uma solicitação SetUserOofSettings ou GetUserOofSettings.  <br/><br/>  A seguir estão as expressões XPath para este elemento: <br/> <br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é opcional. Veja a seguir os valores possíveis:

* SMTP
* EX

Se nenhum valor for fornecido, o valor padrão de SMTP será usado.
  
## <a name="remarks"></a>Comentários

Esse elemento pode ocorrer no máximo uma vez no elemento [email (EmailAddressType)](email-emailaddresstype.md) . Esse elemento não é obrigatório. Esse elemento existe para a inclusão de futuros protocolos. Outro elemento **RoutingType** é usado para acessar itens na caixa de correio de um usuário. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [Obtendo disponibilidade do usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

