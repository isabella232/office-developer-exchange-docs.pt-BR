---
title: mexRuntime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- mexRuntime
api_type:
- schema
ms.assetid: eabb2f12-10a7-4ce2-ae4b-9c04010c765f
description: 'Última modificação: 17 de setembro de 2015'
ms.openlocfilehash: f192965a8375eb46d1ca5b46d3b768a3299c284d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461832"
---
# <a name="mexruntime"></a>mexRuntime
  
**Aplica-se a:** Exchange Server 2013
  
O elemento **mexRuntime** contém elementos que definem informações de configuração para o monitoramento de agentes e informações de configuração para SMTP e agentes de roteamento instalados. 
  
- [configuration](configuration.md)  
- [mexRuntime](mexruntime.md)
  
```XML
<mexRuntime>
   <monitoring/>
   <agentList/>
</mexRuntime>
```

**mexRuntimeType (complexType)**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[monitoramento](monitoring.md) <br/> |Contém informações de configuração que definem como e quando o transporte monitora agentes instalados.  <br/> |
|[agentlist](agentlist.md) <br/> |Contém um elemento [Agent](agent.md) para cada agente instalado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[configuration](configuration.md) <br/> |O elemento raiz para o arquivo de configuração dos agentes.  <br/> |
   
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |Este arquivo não define um namespace.  <br/> |
|Nome do esquema  <br/> |Indisponível.  <br/> |
|Arquivo de validação  <br/> |Indisponível.  <br/> |
|Pode ser vazio  <br/> |Falso.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos de arquivo de configuração de agentes para o Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

