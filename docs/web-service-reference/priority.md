---
title: Prioridade
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Priority
api_type:
- schema
ms.assetid: e1adb8b9-e3d5-469a-b188-822733d2503e
description: O elemento Priority indica a ordem na qual uma regra deve ser executado.
ms.openlocfilehash: 6dc31de851d193deea1f47d07590ce21a90fc020
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542999"
---
# <a name="priority"></a>Prioridade

O **elemento Priority** indica a ordem na qual uma regra deve ser executado. 
  
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
|[Rule (RuleType)](rule-ruletype.md) <br/> |Representa uma regra na caixa de correio do usuário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **Priority** é um inteiro que indica a ordem de execução na qual uma regra deve ser executado. 
  
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

