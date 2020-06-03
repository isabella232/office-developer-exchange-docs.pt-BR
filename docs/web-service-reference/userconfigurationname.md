---
title: Userconfigurationname
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
description: O elemento userconfigurationname representa o nome de um objeto de configuração do usuário. O nome do objeto de configuração do usuário é o identificador de um objeto de configuração do usuário.
ms.openlocfilehash: 020b55919f7f81602a5eb072652d82168607d306
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466028"
---
# <a name="userconfigurationname"></a>Userconfigurationname

O elemento **Userconfigurationname** representa o nome de um objeto de configuração do usuário. O nome do objeto de configuração do usuário é o identificador de um objeto de configuração do usuário. 
  
```XML
<UserConfigurationName Name="">
   <FolderId/>
</UserConfigurationName>
```

```XML
<UserConfigurationName Name="">
   <DistinguishedFolderId/> 
</UserConfigurationName>
```

**Userconfigurationtype**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Nome** <br/> |Contém um valor String que representa o nome de um objeto de configuração do usuário. Esse atributo é necessário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Representa o identificador de pasta da pasta que contém o objeto de configuração do usuário.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Representa um nome de pasta distinta da pasta que contém o objeto de configuração do usuário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DeleteUserConfiguration](deleteuserconfiguration.md) <br/> |Representa uma solicitação para excluir um objeto de configuração do usuário.  <br/> |
|[GetUserConfiguration](getuserconfiguration.md) <br/> |Representa uma solicitação para obter um objeto de configuração do usuário.  <br/> |
|[Userconfiguration](userconfiguration.md) <br/> |Define um único objeto de configuração do usuário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

