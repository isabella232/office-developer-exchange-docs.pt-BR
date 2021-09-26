---
title: RecipientIs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecipientIs
api_type:
- schema
ms.assetid: 5d2fd7ce-6137-4b3c-a716-c0218dcc8a09
description: O elemento RecipientIs especifica que qualquer destinatário da mensagem de email corresponde a qualquer um dos destinatários especificados nos elementos Value filho (ProtectionRuleValueType).
ms.openlocfilehash: 0bf9d96469c626ddc223b128a6d7fabebbfebc84
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542894"
---
# <a name="recipientis"></a>RecipientIs

O **elemento RecipientIs** especifica que qualquer destinatário da mensagem de email corresponde a qualquer um dos destinatários especificados nos elementos [Value filho (ProtectionRuleValueType).](value-protectionrulevaluetype.md) 
  
```xml
<RecipientIs>   <Value/></RecipientIs>
```

 **ProtectionRuleRecipientIsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) <br/> |Identifica um destinatário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Condition](condition.md) <br/> |Identifica a condição que deve ser atendida para que a parte de ação da regra seja executada.  <br/> |
|[And (ProtectionRuleAndType)](and-protectionruleandtype.md) <br/> |Indica que todos os elementos filho devem corresponder para avaliar como **true**.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2010 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

