---
title: GroupSids
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GroupSids
api_type:
- schema
ms.assetid: ebb00653-83f0-4080-a902-c38df6719800
description: O elemento GroupSids representa uma coleção de identificadores de segurança de objeto do grupo de serviços do Active Directory.
ms.openlocfilehash: 9dde1c87a82dbef2a9e1278de2cc202189f309c7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539672"
---
# <a name="groupsids"></a>GroupSids

O **elemento GroupSids** representa uma coleção de identificadores de segurança de objeto do grupo de serviços do Active Directory. 
  
```xml
<GroupSids>
   <GroupIdentifier/>
</GroupSids>
```

 **NonEmptyArrayOfGroupIdentifiersType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GroupIdentifier](groupidentifier.md) <br/> |Representa um único identificador e atributo de segurança para um grupo de objetos do Active Directory do qual a conta é membro.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SerializedSecurityContext](serializedsecuritycontext.md) <br/> |Usado no header SOAP (Simple Object Access Protocol) para serialização de token na autenticação de servidor para servidor. Não há suporte para serialização de token.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

