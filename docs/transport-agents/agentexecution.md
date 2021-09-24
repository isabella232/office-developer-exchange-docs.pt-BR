---
title: agentExecution
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- agentExecution
api_type:
- schema
ms.assetid: 600c4690-941c-45af-a906-5528748d09cd
description: 'Última modificação: 17 de setembro de 2015'
ms.openlocfilehash: 04a53e2698c66326943bcd083c775b53f5c6d5d5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513056"
---
# <a name="agentexecution"></a>agentExecution
  
**Aplica-se a:** Exchange Server 2013 
  
O **elemento agentExecution** define o tempo, em milissegundos, para que o servidor de Acesso para Cliente ou Caixa de Correio aguarde o retorno de um agente de um evento antes de ser gravando no log de eventos. 
  
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
|**timeLimitInMilliseconds** <br/> |Um valor inteiro positivo que especifica o tempo, em milissegundos, para que o servidor aguarde o retorno de um agente de um evento antes de escrever um aviso no log de eventos. O desempenho pode diminuir se esse valor for muito pequeno. O valor sugerido para esse atributo é 300.000, o que equivale a 5 minutos.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[monitoramento](monitoring.md) <br/> |Contém informações de configuração que definem como e quando o serviço de Transporte de Front-End ou o serviço de Transporte monitora os agentes instalados.  <br/> |
   
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |Esse arquivo não define um namespace.  <br/> |
|Nome do esquema  <br/> |Indisponível.  <br/> |
|Arquivo de validação  <br/> |Indisponível.  <br/> |
|Pode ser vazio  <br/> |Falso.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos de arquivo de configuração de agentes para Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

