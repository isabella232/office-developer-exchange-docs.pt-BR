---
title: Agente
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agent
api_type:
- schema
ms.assetid: 0bf744a5-9d79-4c82-8ea7-45fdb3f55300
description: 'Última modificação: 17 de setembro de 2015'
ms.openlocfilehash: a810bb229015054e0f244773760235114655a982
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455678"
---
# <a name="agent"></a>Agente
  
**Aplica-se a:** Exchange Server 2013
  
O elemento **Agent** contém informações de configuração sobre um agente instalado. 
  
- [configuration](configuration.md) 
- [mexRuntime](mexruntime.md)
- [agentlist](agentlist.md)
- [Agente](agent.md)
  
```XML
<agent
        name=""
        baseType=""
        classFactory=""
        assemblyPath=""
        enabled="" />
</agent>
```

**AgentType (complexType)**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**name** <br/> |O nome que foi especificado quando o agente foi instalado. Este atributo requer um valor de cadeia de caracteres não vazio que contenha um máximo de 64 caracteres.  <br/> |
|**baseType** <br/> |O nome completo, incluindo o namespace, da classe a partir da qual o agente deriva. Este atributo requer um valor de cadeia de caracteres não vazio que contenha pelo menos um caractere.  <br/> |
|**classFactory** <br/> |O nome completo, incluindo o namespace, da classe que implementa o alocador de agentes que cria instâncias do agente. Este atributo deve conter o nome totalmente qualificado da classe que implementa o alocador de agentes que cria instâncias do agente. Essa classe deve ser derivada da classe [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) ou [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) .  <br/> |
|**assemblyPath** <br/> |O caminho totalmente qualificado, incluindo o nome do arquivo, do assembly que contém o código para o agente. Este atributo requer um valor de cadeia de caracteres não vazio que contenha pelo menos um caractere.  <br/> |
|**enabled** <br/> |Um valor Boolean que indica se o agente está habilitado. O valor será **true** se o agente estiver habilitado; caso contrário, o valor será **false**. Esse atributo é necessário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[agentlist](agentlist.md) <br/> |Contém um elemento **Agent** para cada agente instalado.  <br/> |
   
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |Este arquivo não define um namespace.  <br/> |
|Nome do esquema  <br/> |Indisponível.  <br/> |
|Arquivo de validação  <br/> |Indisponível.  <br/> |
|Pode ser vazio  <br/> |Falso.  <br/> |
   
## <a name="see-also"></a>Também consulte

- [Elementos de arquivo de configuração de agentes para o Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

