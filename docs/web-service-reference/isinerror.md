---
title: IsInError
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsInError
api_type:
- schema
ms.assetid: f56e6c31-a566-4761-8755-d90ffe6fe790
description: O elemento IsInError indica se a regra está em uma condição de erro.
ms.openlocfilehash: 9e642c9f89434bdcad97b0c16dc35f99196051d7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464214"
---
# <a name="isinerror"></a>IsInError

O elemento **IsInError** indica se a regra está em uma condição de erro. 
  
```XML
<IsInError/>
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
|[Regra (RuleType)](rule-ruletype.md) <br/> |Representa uma regra na caixa de correio do usuário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** indica que a regra está em uma condição de erro. Um valor **false** indica que a regra não está em uma condição de erro. 
  
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

