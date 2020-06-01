---
title: ErrorCode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0bb00cee-c66b-4f34-b99d-355458f5e83b
description: O elemento ErrorCode representa um código de erro de validação de regra que descreve o que houve falha na validação de cada predicado ou ação de regra.
ms.openlocfilehash: 6432aeee786d74a9afcb346cb66765f9001257de
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460075"
---
# <a name="errorcode"></a>ErrorCode

O elemento **ErrorCode** representa um código de erro de validação de regra que descreve o que houve falha na validação de cada predicado ou ação de regra. 
  
```XML
<ErrorCode/>
```

 **RuleValidationErrorCodeType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Erro](error.md) <br/> |Representa um único erro de validação em um valor de propriedade de regra específico, um valor da propriedade Predicate ou um valor da propriedade Action.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto para este elemento é restrito a uma das seguintes cadeias de caracteres:
  
- ADOperationFailure
    
- ConnectedAccountNotFound
    
- CreateWithRuleId
    
- EmptyValueFound
    
- DuplicatedPriority
    
- DuplicatedOperationOnTheSameRule
    
- FolderDoesNotExist
    
- InvalidAddress
    
- InvalidDateRange
    
- InvalidFolderId
    
- InvalidSizeRange
    
- Inválidos
    
- MessageClassificationNotFound
    
- Faltandoaction
    
- MissingParameter
    
- MissingRangeValue
    
- Não condefinida
    
- RecipientDoesNotExist
    
- RuleNotFound
    
- SizeLessThanZero
    
- StringValueTooBig
    
- UnsupportedAddress
    
- UnexpectedError
    
- UnsupportedRule
    
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

