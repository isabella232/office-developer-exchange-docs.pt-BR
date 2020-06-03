---
title: Prioridade
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Priority
api_type:
- schema
ms.assetid: e1adb8b9-e3d5-469a-b188-822733d2503e
description: O elemento Priority indica a ordem na qual uma regra deve ser executada.
ms.openlocfilehash: a5a894bba583618dd04430fc89f125c8920b0202
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462399"
---
# <a name="priority"></a>Prioridade

O elemento **Priority** indica a ordem na qual uma regra deve ser executada. 
  
```XML
<Priority/>
```

 **int**
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

O valor de texto para o elemento **Priority** é um inteiro que indica a ordem de execução na qual uma regra deve ser executada. 
  
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

