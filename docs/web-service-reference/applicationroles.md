---
title: ApplicationRoles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 00003b9b-f8f1-4452-a0af-157f789f8892
description: O elemento ApplicationRoles especifica as funções de aplicativo que o aplicativo parceiro de chamada usa para a chamada atual.
ms.openlocfilehash: a2179d37da6f4870f58a9deaf0585d1418d5792a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522072"
---
# <a name="applicationroles"></a>ApplicationRoles

O **elemento ApplicationRoles** especifica as funções de aplicativo que o aplicativo parceiro de chamada usa para a chamada atual. 
  
```XML
<ApplicationRoles>
    <Role></Role>
</ApplicationRoles>
```

 **NonEmptyArrayOfRoleType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Função](role.md) <br/> |Especifica uma cadeia de caracteres que representa uma função de gerenciamento.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ManagementRole](managementrole.md) <br/> |Especifica a função de gerenciamento.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Tipo de esquema  <br/> |
|Arquivo de validação  <br/> |types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

