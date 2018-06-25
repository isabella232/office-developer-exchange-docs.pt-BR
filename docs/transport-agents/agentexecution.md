---
title: agentExecution
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agentExecution
api_type:
- schema
ms.assetid: 600c4690-941c-45af-a906-5528748d09cd
description: 'Modificado pela última vez: 17 de setembro de 2015'
ms.openlocfilehash: 5848d52a68c8c3f747614015e49becb34bc4cfd8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750993"
---
# <a name="agentexecution"></a>agentExecution
  
**Aplica-se a:** Exchange Server 2013 
  
O elemento de **agentExecution** define o tempo, em milissegundos, para o servidor de acesso para cliente ou caixa de correio aguardar um operador retornar a partir de um evento antes que ela foi gravada no log de eventos. 
  
- [configuração](configuration.md)  
- [monitoramento](monitoring.md)
- [agentExecution](agentexecution.md)
  
```XML
<agentExecution timeLimitInMilliseconds="" />
```

**agentExecutionType (complexType)**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**timeLimitInMilliseconds** <br/> |Um valor de número inteiro positivo que especifica o tempo, em milissegundos, para o servidor deverá esperar um operador retornar a partir de um evento antes que ele grava um aviso no log de eventos. O desempenho pode diminuir se esse valor é muito pequeno. O valor sugerido para este atributo é 300.000, que é igual a 5 minutos.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[monitoramento](monitoring.md) <br/> |Contém informações de configuração que define como e quando o serviço Front End Transport ou o serviço de transporte monitora os operadores que estão instalados.  <br/> |
   
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |Esse arquivo não define um namespace.  <br/> |
|Nome do esquema  <br/> |Não disponível.  <br/> |
|Arquivo de validação  <br/> |Não disponível.  <br/> |
|Pode ser vazio  <br/> |Falso.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos de arquivo de configuração de agentes para o Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

