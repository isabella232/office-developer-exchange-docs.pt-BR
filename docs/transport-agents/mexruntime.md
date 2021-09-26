---
title: mexRuntime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- mexRuntime
api_type:
- schema
ms.assetid: eabb2f12-10a7-4ce2-ae4b-9c04010c765f
description: 'Última modificação: 17 de setembro de 2015'
ms.openlocfilehash: c7ae630a01ac0339433a7c78859c06006efab4b5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546907"
---
# <a name="mexruntime"></a>mexRuntime
  
**Aplica-se a:** Exchange Server 2013
  
O **elemento mexRuntime** contém elementos que definem informações de configuração para informações de monitoramento e configuração de agentes para SMTP e agentes de roteamento instalados. 
  
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
|[agentList](agentlist.md) <br/> |Contém um [elemento de](agent.md) agente para cada agente instalado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[configuration](configuration.md) <br/> |O elemento raiz do arquivo de configuração de agentes.  <br/> |
   
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |Esse arquivo não define um namespace.  <br/> |
|Nome do esquema  <br/> |Indisponível.  <br/> |
|Arquivo de validação  <br/> |Indisponível.  <br/> |
|Pode ser vazio  <br/> |Falso.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos de arquivo de configuração de agentes para Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

