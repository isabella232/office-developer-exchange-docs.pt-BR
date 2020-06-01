---
title: Erro
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Error
api_type:
- schema
ms.assetid: b1f54673-578a-496b-99f5-0fde2c669278
description: O elemento error representa um único erro de validação em um valor de propriedade de regra específico, valor da propriedade Predicate ou valor da propriedade Action.
ms.openlocfilehash: 9c28f63aa79446d89152868c81c85ffa7b3a8b39
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460677"
---
# <a name="error"></a>Erro

O elemento **Error** representa um único erro de validação em um valor de propriedade de regra específico, valor da propriedade Predicate ou valor da propriedade Action. 
  
```XML
<Error>
   <FieldUri/>
   <ErrorCode/>
   <ErrorMessage/>
   <FieldValue/>
</Error>
```

 **RuleValidationErrorType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FieldUri (regra)](fielduri-rule.md) <br/> |Especifica o URI para o campo de regra que causou o erro de validação.  <br/> |
|[ErrorCode](errorcode.md) <br/> |Representa um código de erro de validação de regra que descreve o que a validação falhou para cada predicado de regra ou ação.  <br/> |
|[ErrorMessage](errormessage.md) <br/> |Representa o motivo do erro de validação.  <br/> |
|[FieldValue](fieldvalue.md) <br/> |Representa o valor do campo que causou o erro de validação.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ValidationErrors](validationerrors.md) <br/> |Representa uma matriz de erros de validação de regra em cada campo de regra que possui um erro.  <br/> |
   
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
   
## <a name="see-also"></a>Também consulte



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

