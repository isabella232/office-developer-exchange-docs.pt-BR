---
title: monitoring
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- monitoring
api_type:
- schema
ms.assetid: 350d7b46-9260-41a7-8613-3cb8cc1b29a5
description: 'Última modificação: 17 de setembro de 2015'
ms.openlocfilehash: 215737fb43e1dbef9b7dd11baea1d3f922df7d34
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540360"
---
# <a name="monitoring"></a>monitoring
  
**Aplica-se a:** Exchange Server 2013
  
O **elemento de** monitoramento contém informações de configuração que definem como e quando o serviço de transporte front-end ou o serviço de Transporte monitora os agentes instalados. 
  
- [configuration](configuration.md)  
- [mexRuntime](mexruntime.md)  
- [monitoramento](monitoring.md)
  
```XML
<monitoring>
   <agentExecution/>
   <messageSnapshot/>
</monitoring>
```

**monitoringType (complexType)**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[agentExecution](agentexecution.md) <br/> |Define o tempo, em milissegundos, para o Acesso para Cliente ou o servidor de Caixa de Correio aguardar o retorno de um agente de um evento antes de ser gravando no log de eventos.  <br/> |
|[messageSnapshot](messagesnapshot.md) <br/> |Contém um atributo que especifica se o recurso de rastreamento de pipeline está habilitado para o Acesso para Cliente ou o servidor de Caixa de Correio.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[mexRuntime](mexruntime.md) <br/> |Contém elementos que definem informações de configuração para informações de monitoramento e configuração de agentes para SMTP e agentes de roteamento instalados.  <br/> |
   
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |Esse arquivo não define um namespace.  <br/> |
|Nome do esquema  <br/> |Indisponível.  <br/> |
|Arquivo de validação  <br/> |Indisponível.  <br/> |
|Pode ser vazio  <br/> |Falso.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos de arquivo de configuração de agentes para Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

