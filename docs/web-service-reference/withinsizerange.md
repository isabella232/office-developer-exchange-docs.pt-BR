---
title: WithinSizeRange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WithinSizeRange
api_type:
- schema
ms.assetid: 6f98650e-3399-4f87-9b7f-40bf20cdb821
description: O elemento WithinSizeRange especifica os tamanhos mínimo e máximo que as mensagens de entrada devem ter para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 31da5815b70e20c47594da89b0b7ccab87eaf8f3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459739"
---
# <a name="withinsizerange"></a>WithinSizeRange

O elemento **WithinSizeRange** especifica os tamanhos mínimo e máximo que as mensagens de entrada devem ter para que a condição ou exceção seja aplicada. 
  
```XML
<WithinSizeRange>
     <MinimumSize/>
     <MaximumSize/>
</WithinSizeRange>
```

 **RulePredicateSizeRangeType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MinimumSize](minimumsize.md) <br/> |Especifica o tamanho mínimo que uma mensagem deve ter para que a condição ou exceção seja aplicada.  <br/> |
|[MaximumSize](maximumsize.md) <br/> |Especifica o tamanho máximo que uma mensagem deve ter para que a condição ou exceção seja aplicada.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Condições](conditions.md) <br/> |Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.  <br/> |
|[Exceções](exceptions.md) <br/> |Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.  <br/> |
   
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

