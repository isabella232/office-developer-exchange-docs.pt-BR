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
description: O elemento de erro representa um erro de validação única em um valor da propriedade regra específica, o valor da propriedade predicado ou o valor da propriedade action.
ms.openlocfilehash: adb2de56b7610aa92b5bf5b8d43ac22f35021b64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752089"
---
# <a name="error"></a>Erro

O elemento de **erro** representa um erro de validação única em um valor da propriedade regra específica, o valor da propriedade predicado ou o valor da propriedade action. 
  
```XML
<Error>
   <FieldUri/>
   <ErrorCode/>
   <ErrorMessage/>
   <FieldValue/>
</Error>
```

 **RuleValidationErrorType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FieldUri (regra)](fielduri-rule.md) <br/> |Especifica o URI para o campo de regra que causou o erro de validação.  <br/> |
|[ErrorCode](errorcode.md) <br/> |Representa um código de erro de validação de regra que descreve o que falha na validação para cada predicado regra ou ação.  <br/> |
|[ErrorMessage](errormessage.md) <br/> |Representa o motivo para o erro de validação.  <br/> |
|[FieldValue](fieldvalue.md) <br/> |Representa o valor do campo que causou o erro de validação.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ValidationErrors](validationerrors.md) <br/> |Representa uma matriz de erros de validação de regra em cada campo de regra que possui um erro.  <br/> |
   
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

