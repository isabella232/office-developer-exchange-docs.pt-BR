---
title: UserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UserConfiguration
api_type:
- schema
ms.assetid: 1811df99-ca5b-48a3-b160-b3fd70320c34
description: O elemento UserConfiguration define um único objeto de configuração do usuário.
ms.openlocfilehash: 3821cabf777143de4a68d20a90cb78acedcff552
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538552"
---
# <a name="userconfiguration"></a>UserConfiguration

O **elemento UserConfiguration** define um único objeto de configuração do usuário. 
  
```XML
<UserConfiguration>
   <UserConfigurationName/>
   <ItemId/>
   <Dictionary/>
   <XmlData/>
  <BinaryData/>
</UserConfiguration>
```

 **UserConfigurationType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UserConfigurationName](userconfigurationname.md) <br/> |Representa o nome de um objeto de configuração do usuário. Esse elemento deve ser usado ao criar um objeto de configuração do usuário.  <br/> |
|[ItemId](itemid.md) <br/> |Define o identificador de item de objeto de configuração do usuário.  <br/> |
|[Dictionary](dictionary.md) <br/> |Define um conjunto de entradas de propriedade de dicionário para um objeto de configuração do usuário.  <br/> |
|[XmlData](xmldata.md) <br/> |Contém conteúdo da propriedade de dados XML para um objeto de configuração do usuário.  <br/> |
|[BinaryData](binarydata.md) <br/> |Contém conteúdo de propriedade de dados binários para um objeto de configuração do usuário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CreateUserConfiguration](createuserconfiguration.md) <br/> |Representa uma solicitação para criar um objeto de configuração do usuário.  <br/> |
|[GetUserConfigurationResponseMessage](getuserconfigurationresponsemessage.md) <br/> |Representa uma resposta que retorna um objeto de configuração do usuário.  <br/> |
|[UpdateUserConfiguration](updateuserconfiguration.md) <br/> |Representa uma solicitação para atualizar um objeto de configuração do usuário.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

