---
title: UserConfigurationName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfigurationName
api_type:
- schema
ms.assetid: 6947dd03-9727-4379-9b9d-42373fa120c7
description: O elemento UserConfigurationName representa o nome de um objeto de configuração do usuário. O nome de objeto de configuração do usuário é o identificador de um objeto de configuração do usuário.
ms.openlocfilehash: 40580343e92493c3d39b090371708269ec3274b9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837972"
---
# <a name="userconfigurationname"></a>UserConfigurationName

O elemento **UserConfigurationName** representa o nome de um objeto de configuração do usuário. O nome de objeto de configuração do usuário é o identificador de um objeto de configuração do usuário. 
  
```XML
<UserConfigurationName Name="">
   <FolderId/>
</UserConfigurationName>
```

 **UserConfigurationNameType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**Name** <br/> |Contém um valor string que representa o nome de um objeto de configuração do usuário. Este atributo é necessário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Representa o identificador de pasta da pasta que contém o objeto de configuração do usuário.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Representa um nome diferenciado de pasta da pasta que contém o objeto de configuração do usuário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DeleteUserConfiguration](deleteuserconfiguration.md) <br/> |Representa uma solicitação para excluir um objeto de configuração do usuário.  <br/> |
|[GetUserConfiguration](getuserconfiguration.md) <br/> |Representa uma solicitação para obter um objeto de configuração do usuário.  <br/> |
|[UserConfiguration](userconfiguration.md) <br/> |Define um objeto de configuração de usuário único.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

