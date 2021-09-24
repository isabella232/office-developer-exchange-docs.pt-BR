---
title: UserRoles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: be003e12-3496-468d-a61c-48af0b819654
description: O elemento UserRoles especifica as funções de usuário que o usuário de chamada ou o usuário que o aplicativo parceiro de chamada está agindo como, deseja aplicar-se à chamada atual.
ms.openlocfilehash: c861cda9a010e909c9ecc5303ddc637a14bcb824
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514974"
---
# <a name="userroles"></a>UserRoles

O **elemento UserRoles** especifica as funções de usuário que o usuário de chamada ou o usuário que o aplicativo parceiro de chamada está agindo como, deseja aplicar-se à chamada atual. 
  
```XML
<UserRoles>
   <Role/>
</UserRoles>
```

 **NonEmptyArrayOfRoleType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[Função](role.md)
  
### <a name="parent-elements"></a>Elementos pai

[ManagementRole](managementrole.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

