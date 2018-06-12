---
title: IsPermissionControlled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsPermissionControlled
api_type:
- schema
ms.assetid: a2fd0340-f31f-4389-a1cd-7e93b40bb3c6
description: O elemento IsPermissionControlled indica se as mensagens recebidas devem ser controlado de permissão (protegida por RMS) na ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: fdd9910b8c35d9d57e724d6fec57d203f38f0359
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824088"
---
# <a name="ispermissioncontrolled"></a>IsPermissionControlled

O elemento **IsPermissionControlled** indica se as mensagens recebidas devem ser controlado de permissão (protegida por RMS) na ordem para a condição ou uma exceção a ser aplicado. 
  
```XML
<IsPermissionControlled>true | false</IsPermissionControlled>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Condições](conditions.md) <br/> |Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.  <br/> |
|[Exceções](exceptions.md) <br/> |Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.  <br/> |
   
## <a name="text-value"></a>Text value

Um valor de texto de **true** indica que a mensagem deve ser RMS protegidos em ordem para a condição ou uma exceção a ser aplicado. Um valor **false** indica que a mensagem não deve ser RMS protegidos em ordem para a condição ou uma exceção a ser aplicado. 
  
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

