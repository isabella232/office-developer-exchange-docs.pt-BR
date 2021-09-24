---
title: Erro
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Error
api_type:
- schema
ms.assetid: b1f54673-578a-496b-99f5-0fde2c669278
description: O elemento Error representa um único erro de validação em um determinado valor de propriedade de regra, valor da propriedade predicado ou valor da propriedade action.
ms.openlocfilehash: aeeda25ccc3e657e99bd6f2fea12322fdd3e720d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530858"
---
# <a name="error"></a>Erro

O **elemento Error** representa um único erro de validação em um determinado valor de propriedade de regra, valor da propriedade predicado ou valor da propriedade action. 
  
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
|[FieldUri (Rule)](fielduri-rule.md) <br/> |Especifica o URI para o campo de regra que causou o erro de validação.  <br/> |
|[ErrorCode](errorcode.md) <br/> |Representa um código de erro de validação de regra que descreve o que falhou na validação para cada predicado de regra ou ação.  <br/> |
|[ErrorMessage](errormessage.md) <br/> |Representa o motivo do erro de validação.  <br/> |
|[FieldValue](fieldvalue.md) <br/> |Representa o valor do campo que causou o erro de validação.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ValidationErrors](validationerrors.md) <br/> |Representa uma matriz de erros de validação de regra em cada campo de regra que tem um erro.  <br/> |
   
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

