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
description: 'Modificado pela última vez: 17 de setembro de 2015'
ms.openlocfilehash: 1b5484467def0bf3d22ba0707357977d5ed461ff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751023"
---
# <a name="monitoring"></a>monitoramento
  
**Aplica-se a:** Exchange Server 2013
  
O elemento de **monitoramento** contém informações de configuração que definem como e quando o serviço de transporte de Front-End ou o serviço de transporte monitora os operadores que estão instalados. 
  
- [configuração](configuration.md)  
- [mexRuntime](mexruntime.md)  
- [monitoramento](monitoring.md)
  
```XML
<monitoring>
   <agentExecution/>
   <messageSnapshot/>
</monitoring>
```

**monitoringType (complexType)**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[agentExecution](agentexecution.md) <br/> |Define o tempo, em milissegundos, para o acesso do cliente ou o servidor de caixa de correio aguardar um operador retornar a partir de um evento antes que ela foi gravada no log de eventos.  <br/> |
|[messageSnapshot](messagesnapshot.md) <br/> |Contém um atributo que especifica se o recurso de rastreamento de pipeline está habilitado para o acesso do cliente ou no servidor de caixa de correio.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[mexRuntime](mexruntime.md) <br/> |Contém os elementos que definem as informações de configuração de monitoramento de agente e informações de configuração de SMTP e os agentes de roteamento que estão instalados.  <br/> |
   
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |Esse arquivo não define um namespace.  <br/> |
|Nome do esquema  <br/> |Não disponível.  <br/> |
|Arquivo de validação  <br/> |Não disponível.  <br/> |
|Pode ser vazio  <br/> |Falso.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos de arquivo de configuração de agentes para o Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

