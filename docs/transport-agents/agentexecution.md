---
title: agentExecution
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agentExecution
api_type:
- schema
ms.assetid: 600c4690-941c-45af-a906-5528748d09cd
description: 'Última modificação: 17 de setembro de 2015'
ms.openlocfilehash: 457257e59fb37659daf2f91b0fa5dfced5c48c03
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44446487"
---
# <a name="agentexecution"></a>agentExecution
  
**Aplica-se a:** Exchange Server 2013 
  
O elemento **agentExecution** define o tempo, em milissegundos, para o servidor de acesso para cliente ou caixa de correio aguardar que um agente retorne de um evento antes de gravar no log de eventos. 
  
- [configuration](configuration.md)  
- [monitoramento](monitoring.md)
- [agentExecution](agentexecution.md)
  
```XML
<agentExecution timeLimitInMilliseconds="" />
```

**agentExecutionType (complexType)**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**timeLimitInMilliseconds** <br/> |Um valor inteiro positivo que especifica o tempo, em milissegundos, para que o servidor aguarde um agente retornar de um evento antes de gravar um aviso no log de eventos. O desempenho pode diminuir se esse valor for muito pequeno. O valor sugerido para este atributo é 300.000, que é igual a 5 minutos.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[monitoramento](monitoring.md) <br/> |Contém informações de configuração que definem como e quando o serviço de transporte de front-end ou o serviço de transporte monitora agentes instalados.  <br/> |
   
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |Este arquivo não define um namespace.  <br/> |
|Nome do esquema  <br/> |Indisponível.  <br/> |
|Arquivo de validação  <br/> |Indisponível.  <br/> |
|Pode ser vazio  <br/> |Falso.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos de arquivo de configuração de agentes para o Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

