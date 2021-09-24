---
title: Name (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Name
api_type:
- schema
ms.assetid: c719c55f-d625-4e64-846f-50ac91881443
description: O elemento Name representa o nome de exibição do usuário da caixa de correio.
ms.openlocfilehash: d62dc16beadd97aaa7b27db7d524507d14cef7bf
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539294"
---
# <a name="name-emailaddress"></a>Name (EmailAddress)

O **elemento Name** representa o nome de exibição do usuário da caixa de correio. 
  
```xml
<Name/>
```

**String**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Email (EmailAddressType)](email-emailaddresstype.md) <br/> |Representa o usuário da caixa de correio para uma consulta GetUserAvailability.  <br/> <br/>Veja a seguir o XPath para este elemento:  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[Mailbox (Availability)](mailbox-availability.md) <br/> | Representa o usuário da caixa de correio para uma solicitação SetUserOofSettings ou GetUserOofSettings.  <br/><br/>  Veja a seguir as expressões XPath para este elemento:  <br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto será necessário se esse elemento for usado.
  
## <a name="remarks"></a>Comentários

Esse elemento pode ocorrer no máximo uma vez no [elemento Email (EmailAddressType).](email-emailaddresstype.md) Esse elemento não é necessário. 
  
> [!NOTE]
> O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente. 
  
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

