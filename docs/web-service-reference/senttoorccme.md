---
title: SentToOrCcMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SentToOrCcMe
api_type:
- schema
ms.assetid: ca43e05d-df37-485b-9276-34678025f2b7
description: O elemento SentToOrCcMe indica se o proprietário da caixa de correio precisa estar em uma propriedade ToRecipients ou CcRecipients de mensagens de entrada para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 0e9dddf53c2b671613a5a4c20e3b845a5d38c247
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510887"
---
# <a name="senttoorccme"></a>SentToOrCcMe

O **elemento SentToOrCcMe** indica se o proprietário da caixa de correio precisa estar em uma **propriedade ToRecipients** ou **CcRecipients** de mensagens de entrada para que a condição ou exceção seja aplicada. 
  
```XML
<SentToOrCcMe>true | false</SentToOrCcMe>
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
|[Exceções](exceptions.md) <br/> |Representa todas as condições de exceção de regra disponíveis para uma regra de Caixa de Entrada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor  de texto true indica que o proprietário da caixa de correio deve estar na **propriedade ToRecipients** ou **CcRecipients** das mensagens de entrada para que a condição ou exceção seja aplicada. Um valor **false** indica que o proprietário da caixa de correio não deve estar na **propriedade ToRecipients** ou **CcRecipients** das mensagens de entrada para que a condição ou exceção seja aplicada. 
  
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

