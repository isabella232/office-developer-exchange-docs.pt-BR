---
title: ErrorCode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0bb00cee-c66b-4f34-b99d-355458f5e83b
description: O elemento ErrorCode representa um código de erro de validação de regra que descreve o que falhou na validação de cada predicado ou ação de regra.
ms.openlocfilehash: a582b09a579074a6728bb79b351b8c7a120c05de
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517109"
---
# <a name="errorcode"></a>ErrorCode

O **elemento ErrorCode** representa um código de erro de validação de regra que descreve o que falhou na validação de cada predicado ou ação de regra. 
  
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
|[Erro](error.md) <br/> |Representa um único erro de validação em um determinado valor de propriedade de regra, valor da propriedade predicado ou valor da propriedade action.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto para esse elemento é restrito a uma das seguintes cadeias de caracteres:
  
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
    
- InvalidValue
    
- MessageClassificationNotFound
    
- MissingAction
    
- MissingParameter
    
- MissingRangeValue
    
- NotSettable
    
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

