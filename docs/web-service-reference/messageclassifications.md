---
title: MessageClassifications
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MessageClassifications
api_type:
- schema
ms.assetid: 041b3d48-8f43-47f3-869f-72b66bef372a
description: O elemento MessageClassifications representa as classificações de mensagem que devem ser carimbadas em mensagens de entrada para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 88ccd4be40d66de2fec859de67aa0e365f451bd4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542082"
---
# <a name="messageclassifications"></a>MessageClassifications

O **elemento MessageClassifications** representa as classificações de mensagem que devem ser carimbadas em mensagens de entrada para que a condição ou exceção seja aplicada. 
  
```XML
<MessageClassifications>
    <String/>
</MessageClassifications>
```

 **ArrayOfStringsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhuma
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[String](string.md) <br/> |Representa uma classificação de mensagem.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Condições](conditions.md) <br/> |Representa as condições que, quando cumpridas, dispararão as ações de regra para uma regra.  <br/> |
|[Exceções](exceptions.md) <br/> |Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de Caixa de Entrada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
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

