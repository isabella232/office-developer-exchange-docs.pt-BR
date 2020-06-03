---
title: Caixa de correio (disponibilidade)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Mailbox
api_type:
- schema
ms.assetid: affd192e-8914-473f-9098-d9bdf898de2c
description: O elemento Mailbox representa o usuário de caixa de correio de uma solicitação SetUserOofSettings ou GetUserOofSettings.
ms.openlocfilehash: 1bda6e8b90551b86b4e1c2711ac25693a65e5410
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458072"
---
# <a name="mailbox-availability"></a>Caixa de correio (disponibilidade)

O elemento **Mailbox** representa o usuário de caixa de correio de uma solicitação SetUserOofSettings ou GetUserOofSettings. 
  
```xml
<Mailbox>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Mailbox>
```

**EmailAddresstype**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Nome (EmailAddress)](name-emailaddress.md) <br/> |Representa o nome de exibição do usuário da caixa de correio. Este elemento é opcional no SetUserOofSettingsRequest. O GetUserOofSettingsRequest retornará este elemento.  <br/> |
|[Endereço (cadeia de caracteres)](address-string.md) <br/> |Representa o endereço de email do usuário da caixa de correio. Este elemento é obrigatório.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Representa o protocolo de roteamento para a mensagem. Este elemento é opcional no SetUserOofSettingsRequest. O GetUserOofSettingsRequest retornará este elemento.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetUserOofSettingsRequest](getuseroofsettingsrequest.md) <br/> |Usado para obter as configurações e mensagens de ausência temporária (OOF) de um usuário de caixa de correio.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/GetUserOofSettingsRequest` <br/> |
|[SetUserOofSettingsRequest](setuseroofsettingsrequest.md) <br/> |Usado para definir as configurações e mensagens de ausência temporária de um usuário de caixa de correio.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a>Comentários

O endereço de email é usado para identificar a pasta de calendário que contém as configurações de ausência temporária. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserOofSettings](getuseroofsettings-operation.md)
- [Operação SetUserOofSettings](setuseroofsettings-operation.md)

