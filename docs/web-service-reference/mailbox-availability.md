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
description: O elemento de caixa de correio representa o usuário de caixa de correio para um SetUserOofSettings ou GetUserOofSettings solicitação.
ms.openlocfilehash: 2e901ae0df56542f56f247184254294735018468
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824254"
---
# <a name="mailbox-availability"></a>Caixa de correio (disponibilidade)

O elemento de **caixa de correio** representa o usuário de caixa de correio para um SetUserOofSettings ou GetUserOofSettings solicitação. 
  
```xml
<Mailbox>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Mailbox>
```

**EmailAddressType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Nome (EmailAddress)](name-emailaddress.md) <br/> |Representa o nome de exibição do usuário da caixa de correio. Esse elemento é opcional a SetUserOofSettingsRequest. O GetUserOofSettingsRequest retornará esse elemento.  <br/> |
|[Endereço (string)](address-string.md) <br/> |Representa o endereço de email do usuário da caixa de correio. Este elemento é obrigatório.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Representa o protocolo de roteamento para a mensagem. Esse elemento é opcional a SetUserOofSettingsRequest. O GetUserOofSettingsRequest retornará esse elemento.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetUserOofSettingsRequest](getuseroofsettingsrequest.md) <br/> |Usado para fazer configurações de fora do escritório (OOF) e mensagens de um usuário de caixa de correio.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/GetUserOofSettingsRequest` <br/> |
|[SetUserOofSettingsRequest](setuseroofsettingsrequest.md) <br/> |Usada para definir configurações de ausência temporária e mensagens de um usuário de caixa de correio.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a>Coment�rios

O endereço de email é usado para identificar a pasta de calendário que contém as configurações de ausência temporária. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação GetUserOofSettings](getuseroofsettings-operation.md)
- [Operação SetUserOofSettings](setuseroofsettings-operation.md)

