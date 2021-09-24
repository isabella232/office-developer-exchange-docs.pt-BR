---
title: agente
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- agent
api_type:
- schema
ms.assetid: 0bf744a5-9d79-4c82-8ea7-45fdb3f55300
description: 'Última modificação: 17 de setembro de 2015'
ms.openlocfilehash: 8bcfdd9bffd4c7a15af40528fd431a99c7868637
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520960"
---
# <a name="agent"></a>agente
  
**Aplica-se a:** Exchange Server 2013
  
O **elemento agent** contém informações de configuração sobre um agente instalado. 
  
- [configuration](configuration.md) 
- [mexRuntime](mexruntime.md)
- [agentList](agentlist.md)
- [agent](agent.md)
  
```XML
<agent
        name=""
        baseType=""
        classFactory=""
        assemblyPath=""
        enabled="" />
</agent>
```

**agentType (complexType)**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**name** <br/> |O nome que foi especificado quando o agente foi instalado. Esse atributo requer um valor de cadeia de caracteres semmpty que contém no máximo 64 caracteres.  <br/> |
|**baseType** <br/> |O nome completo, incluindo o namespace, da classe da qual o agente deriva. Esse atributo requer um valor de cadeia de caracteres semmpty que contém pelo menos um caractere.  <br/> |
|**classFactory** <br/> |O nome completo, incluindo o namespace, da classe que implementa a fábrica de agentes que cria instâncias do agente. Esse atributo deve conter o nome totalmente qualificado da classe que implementa a fábrica de agentes que cria instâncias do agente. Essa classe deve derivar da [classe SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) ou [RoutingAgentFactory.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)  <br/> |
|**assemblyPath** <br/> |O caminho totalmente qualificado, incluindo o nome do arquivo, do assembly que contém o código do agente. Esse atributo requer um valor de cadeia de caracteres semmpty que contém pelo menos um caractere.  <br/> |
|**enabled** <br/> |Um valor Boolean que indica se o agente está habilitado. O valor será **true** se o agente estiver habilitado; caso contrário, o valor será **false**. Esse atributo é necessário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[agentList](agentlist.md) <br/> |Contém um **elemento de** agente para cada agente instalado.  <br/> |
   
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |Esse arquivo não define um namespace.  <br/> |
|Nome do esquema  <br/> |Indisponível.  <br/> |
|Arquivo de validação  <br/> |Indisponível.  <br/> |
|Pode ser vazio  <br/> |Falso.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos de arquivo de configuração de agentes para Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

