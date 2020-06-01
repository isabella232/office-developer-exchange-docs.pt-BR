---
title: Email (EmailAddresstype)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Email
api_type:
- schema
ms.assetid: dfffa1d5-2c3c-4f56-af63-5853df462e58
description: O elemento email representa o usuário de caixa de correio de uma consulta GetUserAvailability.
ms.openlocfilehash: 2ed8de9c011a385ec6c4ebd2f8d1d47304343a0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459227"
---
# <a name="email-emailaddresstype"></a>Email (EmailAddresstype)

O elemento **email** representa o usuário de caixa de correio de uma consulta GetUserAvailability. 
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)  
- [MailboxDataArray](mailboxdataarray.md) 
- [MailboxData](mailboxdata.md) 
- [Email (EmailAddresstype)](email-emailaddresstype.md)
  
```xml
<Email>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Email>
```

 **EmailAddresstype**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Nome (EmailAddress)](name-emailaddress.md) <br/> |Representa o nome de exibição do usuário da caixa de correio.  <br/> |
|[Endereço (cadeia de caracteres)](address-string.md) <br/> |Representa o endereço de email do usuário da caixa de correio.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Representa o protocolo de roteamento para a mensagem.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MailboxData](mailboxdata.md) <br/> |Representa um usuário de caixa de correio individual e opções para o tipo de dados a ser retornado sobre o usuário da caixa de correio.  <br/> Este é o XPath para este elemento:  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório/EWS/do computador que está executando o MicrosoftExchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
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

