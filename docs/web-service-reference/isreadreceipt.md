---
title: IsReadReceipt
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsReadReceipt
api_type:
- schema
ms.assetid: e60e525f-c136-469a-b68b-b3dc01f400a6
description: O elemento IsReadReceipt indica se as mensagens de entrada devem ser recibos de leitura para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 65ed10e4bc3fa38aed0566e672d57ec720556b94
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514470"
---
# <a name="isreadreceipt"></a>IsReadReceipt

O **elemento IsReadReceipt** indica se as mensagens de entrada devem ser recibos de leitura para que a condição ou exceção seja aplicada. 
  
```XML
<IsReadReceipt> true | false</IsReadReceipt>
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
|[Condições](conditions.md) <br/> |Representa as condições que, quando cumpridas, dispararão as ações de regra para essa regra.  <br/> |
|[Exceções](exceptions.md) <br/> |Representa todas as condições de exceção de regra disponíveis para a regra caixa de entrada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** indica que a mensagem deve ser um recibo de leitura para que a condição ou exceção seja aplicada. Se a mensagem não precisa ser um recibo de leitura para que a condição ou exceção seja aplicada, o valor será **false**.
  
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

