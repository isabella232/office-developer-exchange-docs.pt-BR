---
title: And (ProtectionRuleAndType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- And
api_type:
- schema
ms.assetid: 7fafd1c8-cd29-43a0-b383-f6595f934f48
description: O elemento And especifica que todos os elementos filho devem corresponder para avaliar como true.
ms.openlocfilehash: 01721b460d87d3282a1a793966b0259e0f1342dd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518935"
---
# <a name="and-protectionruleandtype"></a>And (ProtectionRuleAndType)

O **elemento And** especifica que todos os elementos filho devem corresponder para avaliar como **true**.
  
```xml
<And>
   <AllInternal/>
   <And/>
   <RecipientIs/>
   <SenderDepartments/>
   <True/>
</And>
```

 **ProtectionRuleAndType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AllInternal](allinternal.md) <br/> |Avalia como **true se** todos os destinatários de uma mensagem de email são internos para a organização do remetente.  <br/> |
|**And** <br/> |Especifica que todos os elementos filho devem corresponder para avaliar como **true**.  <br/> |
|[RecipientIs](recipientis.md) <br/> |Especifica que qualquer destinatário da mensagem de email corresponde a qualquer um dos destinatários especificados nos elementos [Child Value (ProtectionRuleValueType).](value-protectionrulevaluetype.md)  <br/> |
|[SenderDepartments](senderdepartments.md) <br/> |Especifica que o departamento do remetente corresponde a qualquer um dos departamentos especificados nos elementos [Child Value (ProtectionRuleValueType).](value-protectionrulevaluetype.md)  <br/> |
|[Verdadeiro](true.md) <br/> |Especifica uma condição que sempre corresponde.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Condition](condition.md) <br/> |Identifica a condição que deve ser atendida para que a parte de ação da regra seja executada.  <br/> |
|**And** <br/> |Especifica que todos os elementos filho devem corresponder para avaliar como **true**.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

