---
title: RoutingType (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RoutingType
api_type:
- schema
ms.assetid: 74d83198-0d9d-4c78-a2bc-9a671859ff37
description: O elemento RoutingType representa o protocolo de roteamento do destinatário.
ms.openlocfilehash: cc4d18ff9fa18f0ec2024f15cb6a3bd4199832de
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534426"
---
# <a name="routingtype-emailaddress"></a>RoutingType (EmailAddress)

O **elemento RoutingType** representa o protocolo de roteamento do destinatário. 
  
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
|[Email (EmailAddressType)](email-emailaddresstype.md) <br/> |Especifica o endereço de email do objeto MailboxData. Esse elemento é usado na operação [GetUserAvailability](getuseravailability-operation.md).  <br/><br/> Veja a seguir o XPath para este elemento:  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[Mailbox (Availability)](mailbox-availability.md) <br/> | Representa o usuário da caixa de correio para uma solicitação SetUserOofSettings ou GetUserOofSettings.  <br/><br/>  Veja a seguir as expressões XPath para este elemento: <br/> <br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é opcional. Veja a seguir os valores possíveis:

* SMTP
* EX

Se nenhum valor for fornecido, o valor padrão de SMTP será usado.
  
## <a name="remarks"></a>Comentários

Esse elemento pode ocorrer no máximo uma vez no [elemento Email (EmailAddressType).](email-emailaddresstype.md) Esse elemento não é necessário. Esse elemento existe para a inclusão de protocolos futuros. Outro **elemento RoutingType** é usado para acessar itens na caixa de correio de um usuário. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [Obter Disponibilidade do Usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

