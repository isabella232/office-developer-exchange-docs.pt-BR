---
title: IsSigned
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsSigned
api_type:
- schema
ms.assetid: a4f90fe5-2834-4621-9aa3-b561f74d4674
description: O elemento IsSigned indica se as mensagens de entrada devem ser assinadas para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 556b5a723a3201721651000264274ebd0cd001e1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524088"
---
# <a name="issigned"></a>IsSigned

O **elemento IsSigned** indica se as mensagens de entrada devem ser assinadas para que a condição ou exceção seja aplicada. 
  
```XML
<IsSigned>true | false</IsSigned>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Condições](conditions.md) <br/> |Representa as condições que, quando cumpridas, dispararão as ações de regra para uma regra.  <br/> |
|[Exceções](exceptions.md) <br/> |Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de Caixa de Entrada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** indica que a mensagem deve ser assinada para que a condição ou exceção seja aplicada. Um valor de texto **false** indica que a mensagem não precisa ser assinada para que a condição ou exceção seja aplicada. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

