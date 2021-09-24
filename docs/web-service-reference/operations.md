---
title: Operações
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Operations
api_type:
- schema
ms.assetid: d8cd41b1-28ae-4c95-9ff6-8b25c8e18306
description: O elemento Operations contém uma matriz de operações de regra que podem ser executadas em uma Caixa de Entrada.
ms.openlocfilehash: 48679c9c7c0482ab53d3af5c661dc6efe513e637
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518068"
---
# <a name="operations"></a>Operações

O **elemento Operations** contém uma matriz de operações de regra que podem ser executadas em uma Caixa de Entrada. 
  
[UpdateInboxRules](updateinboxrules.md)
  
```XML
<Operations>
    <CreateRuleOperation/>
    <SetRuleOperation/>
    <DeleteRuleOperation/>
</Operations>
```

 **ArrayOfRuleOperationsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CreateRuleOperation](createruleoperation.md) <br/> |Representa uma operação para criar uma nova regra de Caixa de Entrada.  <br/> |
|[SetRuleOperation](setruleoperation.md) <br/> |Representa uma operação para atualizar uma regra de Caixa de Entrada.  <br/> |
|[DeleteRuleOperation](deleteruleoperation.md) <br/> |Representa uma operação para excluir uma regra de Caixa de Entrada.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UpdateInboxRules](updateinboxrules.md) <br/> |Define uma solicitação para atualizar as regras de Caixa de Entrada em uma caixa de correio no armazenamento do servidor.  <br/> |
   
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



[Operação UpdateInboxRules](updateinboxrules-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

