---
title: ApplicationRoles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00003b9b-f8f1-4452-a0af-157f789f8892
description: O elemento ApplicationRoles Especifica as funções do aplicativo usados pelo aplicativo de parceiro a chamada para a chamada atual.
ms.openlocfilehash: ff32b693dae573416263bcb7c0fbb552a933b8d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751102"
---
# <a name="applicationroles"></a>ApplicationRoles

O elemento **ApplicationRoles** Especifica as funções do aplicativo usados pelo aplicativo de parceiro a chamada para a chamada atual. 
  
```XML
<ApplicationRoles>
    <Role></Role>
</ApplicationRoles>
```

 **NonEmptyArrayOfRoleType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Role](role.md) <br/> |Especifica uma cadeia de caracteres que representa uma função de gerenciamento.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ManagementRole](managementrole.md) <br/> |Especifica a função de gerenciamento.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

