---
title: Endereço (cadeia de caracteres)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Address
api_type:
- schema
ms.assetid: a3cdfcbd-d0c5-46d6-8daa-52405fc63ff0
description: O elemento address representa o endereço de email do usuário da caixa de correio.
ms.openlocfilehash: 839107050f22df5c00cb4dea9c531563df52933d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463640"
---
# <a name="address-string"></a>Endereço (cadeia de caracteres)

O elemento **Address** representa o endereço de email do usuário da caixa de correio. 
  
```xml
<Address>...</Address>
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
|[Email (EmailAddresstype)](email-emailaddresstype.md) <br/> |Especifica o endereço de email do objeto MailboxData. Este elemento é usado na [operação GetUserAvailability](getuseravailability-operation.md).<br/><br/> Este é o XPath para este elemento:<br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[Caixa de correio (disponibilidade)](mailbox-availability.md) <br/> | Representa o usuário de caixa de correio de uma solicitação SetUserOofSettings ou GetUserOofSettings.<br/><br/>  A seguir estão as expressões XPath para este elemento:<br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto será necessário se esse elemento for usado.
  
## <a name="remarks"></a>Comentários

Esse elemento pode ocorrer no máximo uma vez no elemento [email (EmailAddressType)](email-emailaddresstype.md) e no elemento [Mailbox (disponibilidade)](mailbox-availability.md) . 
  
> [!NOTE]
> O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserAvailability](getuseravailability-operation.md)
- [Operação GetUserOofSettings](getuseroofsettings-operation.md)
- [Operação SetUserOofSettings](setuseroofsettings-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [GetUserOofSettingsRequest](getuseroofsettingsrequest.md)
- [SetUserOofSettingsRequest](setuseroofsettingsrequest.md)
- [Obtendo disponibilidade do usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

