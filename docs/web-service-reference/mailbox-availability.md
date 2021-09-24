---
title: Mailbox (Availability)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Mailbox
api_type:
- schema
ms.assetid: affd192e-8914-473f-9098-d9bdf898de2c
description: O elemento Mailbox representa o usuário da caixa de correio para uma solicitação SetUserOofSettings ou GetUserOofSettings.
ms.openlocfilehash: 5e32c4be807dae92b27df7012caa8eb1b295b26c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522919"
---
# <a name="mailbox-availability"></a>Mailbox (Availability)

O **elemento Mailbox** representa o usuário da caixa de correio para uma solicitação SetUserOofSettings ou GetUserOofSettings. 
  
```xml
<Mailbox>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Mailbox>
```

**EmailAddressType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Name (EmailAddress)](name-emailaddress.md) <br/> |Representa o nome de exibição do usuário da caixa de correio. Esse elemento é opcional no SetUserOofSettingsRequest. GetUserOofSettingsRequest retornará esse elemento.  <br/> |
|[Address (string)](address-string.md) <br/> |Representa o endereço de email do usuário da caixa de correio. Este elemento é obrigatório.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Representa o protocolo de roteamento da mensagem. Esse elemento é opcional no SetUserOofSettingsRequest. GetUserOofSettingsRequest retornará esse elemento.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetUserOofSettingsRequest](getuseroofsettingsrequest.md) <br/> |Usado para obter mensagens e configurações de um usuário de caixa de correio fora do Office (OOF).  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/GetUserOofSettingsRequest` <br/> |
|[SetUserOofSettingsRequest](setuseroofsettingsrequest.md) <br/> |Usado para definir as configurações e mensagens OOF de um usuário de caixa de correio.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a>Comentários

O endereço de email é usado para identificar a pasta de calendário que contém as configurações OOF. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserOofSettings](getuseroofsettings-operation.md)
- [Operação SetUserOofSettings](setuseroofsettings-operation.md)

