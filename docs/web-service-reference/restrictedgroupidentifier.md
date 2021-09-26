---
title: RestrictedGroupIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RestrictedGroupIdentifier
api_type:
- schema
ms.assetid: a3ea3c81-9f99-4836-8cb4-2384ea63f093
description: O elemento RestrictGroupIdentifier representa o SID (identificador de segurança do grupo) e os atributos de um grupo restrito dentro de um token de usuário.
ms.openlocfilehash: 65b356f4a8195979d751a3f5288940b391f51939
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544777"
---
# <a name="restrictedgroupidentifier"></a>RestrictedGroupIdentifier

O **elemento RestrictGroupIdentifier** representa o SID (identificador de segurança do grupo) e os atributos de um grupo restrito dentro de um token de usuário. 
  
```xml
<RestrictedGroupIdentifier Attributes="">
   <SecurityIdentifier/>
</RestrictedGroupIdentifier>
```

 **SidAndAttributesType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Atributos** <br/> |Contém atributos de grupo.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SecurityIdentifier](securityidentifier.md) <br/> |Representa o formulário SDDL (linguagem de definição de descritor de segurança) de um identificador de segurança.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RestrictedGroupSids](restrictedgroupsids.md) <br/> |Representa uma coleção de grupos restritos dentro de um token de usuário. Não há suporte para serialização de token.  <br/> |
   
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

