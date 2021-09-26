---
title: StopProcessingRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StopProcessingRules
api_type:
- schema
ms.assetid: 5b89a2cb-ab26-444d-b3dd-2b3858872d63
description: O elemento StopProcessingRules indica se as regras subsequentes devem ser avaliadas.
ms.openlocfilehash: 21eaed44f6a599583e67d770cd783a479e612f87
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545843"
---
# <a name="stopprocessingrules"></a>StopProcessingRules

O **elemento StopProcessingRules** indica se as regras subsequentes devem ser avaliadas. 
  
```XML
<StopProcessingRules>true | false</StopProcessingRules>
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
|[Actions](actions.md) <br/> |Representa o conjunto de ações que estão disponíveis para serem tomadas em uma mensagem quando as condições são atendidas.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** indica que as regras subsequentes não devem ser processadas. Um valor **false** indica que as regras subsequentes devem continuar a ser avaliadas. 
  
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

