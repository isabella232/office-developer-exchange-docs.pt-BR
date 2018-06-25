---
title: Operações
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Operations
api_type:
- schema
ms.assetid: d8cd41b1-28ae-4c95-9ff6-8b25c8e18306
description: O elemento de operações contém uma matriz das operações de regra que podem ser executadas em uma caixa de entrada.
ms.openlocfilehash: 1030703d5e496be391d557e99e1420f9fddfdb36
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824655"
---
# <a name="operations"></a>Operações

O elemento de **operações** contém uma matriz das operações de regra que podem ser executadas em uma caixa de entrada. 
  
[UpdateInboxRules](updateinboxrules.md)
  
```XML
<Operations>
    <CreateRuleOperation/>
    <SetRuleOperation/>
    <DeleteRuleOperation/>
</Operations>
```

 **ArrayOfRuleOperationsType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CreateRuleOperation](createruleoperation.md) <br/> |Representa uma operação para criar uma nova regra de caixa de entrada.  <br/> |
|[SetRuleOperation](setruleoperation.md) <br/> |Representa uma operação de atualização de uma regra de caixa de entrada.  <br/> |
|[DeleteRuleOperation](deleteruleoperation.md) <br/> |Representa uma operação para excluir uma regra de caixa de entrada.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UpdateInboxRules](updateinboxrules.md) <br/> |Define uma solicitação para atualizar as regras de caixa de entrada em uma caixa de correio no armazenamento do servidor.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação UpdateInboxRules](updateinboxrules-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

