---
title: monitoramento
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- monitoring
api_type:
- schema
ms.assetid: 350d7b46-9260-41a7-8613-3cb8cc1b29a5
description: 'Última modificação: 17 de setembro de 2015'
ms.openlocfilehash: 5614ac2c6428da9b6845769a9335486d3ded5754
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455825"
---
# <a name="monitoring"></a>monitoramento
  
**Aplica-se a:** Exchange Server 2013
  
O elemento **Monitoring** contém informações de configuração que definem como e quando o serviço de transporte de front-end ou o serviço de transporte monitora os agentes instalados. 
  
- [configuration](configuration.md)  
- [mexRuntime](mexruntime.md)  
- [monitoramento](monitoring.md)
  
```XML
<monitoring>
   <agentExecution/>
   <messageSnapshot/>
</monitoring>
```

**monitortype (complexType)**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[agentExecution](agentexecution.md) <br/> |Define o tempo, em milissegundos, para o acesso do cliente ou o servidor de caixa de correio para aguardar que um agente retorne de um evento antes de gravar no log de eventos.  <br/> |
|[messageSnapshot](messagesnapshot.md) <br/> |Contém um atributo que especifica se o recurso de rastreamento de pipeline está habilitado para o acesso do cliente ou o servidor de caixa de correio.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[mexRuntime](mexruntime.md) <br/> |Contém elementos que definem informações de configuração para o monitoramento de agentes e informações de configuração para SMTP e agentes de roteamento instalados.  <br/> |
   
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |Este arquivo não define um namespace.  <br/> |
|Nome do esquema  <br/> |Indisponível.  <br/> |
|Arquivo de validação  <br/> |Indisponível.  <br/> |
|Pode ser vazio  <br/> |Falso.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos de arquivo de configuração de agentes para o Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

