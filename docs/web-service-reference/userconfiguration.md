---
title: UserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfiguration
api_type:
- schema
ms.assetid: 1811df99-ca5b-48a3-b160-b3fd70320c34
description: O elemento de UserConfiguration define um objeto de configuração de usuário único.
ms.openlocfilehash: ce3eaa470ef592c5a8e5a7ef24c377bb2feeca2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837973"
---
# <a name="userconfiguration"></a>UserConfiguration

O elemento de **UserConfiguration** define um objeto de configuração de usuário único. 
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UserConfigurationName](userconfigurationname.md) <br/> |Representa o nome de um objeto de configuração do usuário. Este elemento deve ser usado quando você cria um objeto de configuração do usuário.  <br/> |
|[ItemId](itemid.md) <br/> |Define o identificador de item do objeto de configuração do usuário.  <br/> |
|[dicionário](dictionary.md) <br/> |Define um conjunto de entradas de propriedade de dicionário para um objeto de configuração do usuário.  <br/> |
|[Xmldatahttp](xmldata.md) <br/> |Possui conteúdo de propriedade de dados XML para um objeto de configuração do usuário.  <br/> |
|[BinaryData](binarydata.md) <br/> |Contém dados binários conteúdo de propriedade para um objeto de configuração do usuário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CreateUserConfiguration](createuserconfiguration.md) <br/> |Representa uma solicitação para criar um objeto de configuração do usuário.  <br/> |
|[GetUserConfigurationResponseMessage](getuserconfigurationresponsemessage.md) <br/> |Representa uma resposta que retorna um objeto de configuração do usuário.  <br/> |
|[UpdateUserConfiguration](updateuserconfiguration.md) <br/> |Representa uma solicitação para atualizar um objeto de configuração do usuário.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

