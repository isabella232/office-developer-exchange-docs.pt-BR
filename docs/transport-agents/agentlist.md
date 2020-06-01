---
title: agentlist
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agentList
api_type:
- schema
ms.assetid: e877b7ef-e303-4270-964d-8d116ff2a865
description: 'Última modificação: 17 de setembro de 2015'
ms.openlocfilehash: 99e4e24c3bca77c7e7d5f2c59bb21cee1317fed2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44446389"
---
# <a name="agentlist"></a>agentlist
  
**Aplica-se a:** Exchange Server 2013
  
O elemento **agentlist** contém um elemento [Agent](agent.md) para cada agente instalado. 
  
- [configuration](configuration.md)
- [mexRuntime](mexruntime.md)
- [agentlist](agentlist.md)
  
```XML
<agentList>
      <agent/>
</agentList>
```

**agentListType (complexType)**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Agente](agent.md) <br/> |Contém informações de configuração sobre um agente instalado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[mexRuntime](mexruntime.md) <br/> |Contém elementos que definem informações de configuração para o monitoramento de agentes e informações de configuração sobre agentes instalados.  <br/> |
   
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |Este arquivo não define um namespace.  <br/> |
|Nome do esquema  <br/> |Indisponível.  <br/> |
|Arquivo de validação  <br/> |Indisponível.  <br/> |
|Pode ser vazio  <br/> |Falso.  <br/> |
   
## <a name="see-also"></a>Também consulte

- [Elementos de arquivo de configuração de agentes para o Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

