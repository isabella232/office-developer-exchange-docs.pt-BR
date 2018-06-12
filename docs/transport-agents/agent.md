---
title: agente
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
description: 'Modificado pela última vez: 17 de setembro de 2015'
ms.openlocfilehash: 3895095ed4e469cdb9fec489ba6b6e228779a9c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750996"
---
# <a name="agent"></a>agente
  
**Aplica-se a:** Exchange Server 2013
  
O elemento de **agente** contém informações de configuração sobre um agente instalado. 
  
- [configuração](configuration.md) 
- [mexRuntime](mexruntime.md)
- [agentList](agentlist.md)
- [agente](agent.md)
  
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

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**name** <br/> |O nome que foi especificado quando o agente foi instalado. Este atributo requer um valor de cadeia de caracteres vazia que contém um máximo de 64 caracteres.  <br/> |
|**baseType** <br/> |O nome completo, incluindo o namespace, da classe do qual o agente deriva. Este atributo requer um valor de cadeia de caracteres vazia que contém pelo menos um caractere.  <br/> |
|**classFactory** <br/> |O nome completo, incluindo o namespace, da classe que implementa o alocador de agente que cria instâncias do agente. Este atributo deve conter o nome totalmente qualificado da classe que implementa o alocador de agente que cria instâncias do agente. Esta classe deve derivar de classe no [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) ou [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) .  <br/> |
|**assemblyPath** <br/> |O caminho totalmente qualificado, incluindo o nome do arquivo do assembly que contém o código para o agente. Este atributo requer um valor de cadeia de caracteres vazia que contém pelo menos um caractere.  <br/> |
|**habilitado** <br/> |Um valor Boolean que indica se o agente está habilitado. O valor é **true** se o agente estiver habilitado; Caso contrário, o valor é **false**. Este atributo é necessário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[agentList](agentlist.md) <br/> |Contém um elemento de **agente** para cada agente instalado.  <br/> |
   
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |Esse arquivo não define um namespace.  <br/> |
|Nome do esquema  <br/> |Não disponível.  <br/> |
|Arquivo de validação  <br/> |Não disponível.  <br/> |
|Pode ser vazio  <br/> |Falso.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos de arquivo de configuração de agentes para o Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

