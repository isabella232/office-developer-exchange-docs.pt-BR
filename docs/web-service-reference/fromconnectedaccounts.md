---
title: FromConnectedAccounts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FromConnectedAccounts
api_type:
- schema
ms.assetid: d4d7ddd7-078d-4f1a-a26b-22dce0c49f3a
description: O elemento FromConnectedAccounts representa os nomes de conta de email do qual mensagens recebidas precisam ter foram agregados na ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: 426e81bbbe96fb5fb4b36506438dc4af4f560eef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752372"
---
# <a name="fromconnectedaccounts"></a>FromConnectedAccounts

O elemento **FromConnectedAccounts** representa os nomes de conta de email do qual mensagens recebidas precisam ter foram agregados na ordem para a condição ou uma exceção a ser aplicado. 
  
```XML
<FromConnectedAccounts>
    <String/>
</FromConnectedAccounts>
```

 **ArrayOfStringsType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[String](string.md) <br/> |Representa um nome de conta de email do qual mensagens recebidas precisam ter foram agregados na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Condições](conditions.md) <br/> |Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.  <br/> |
|[Exceções](exceptions.md) <br/> |Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

