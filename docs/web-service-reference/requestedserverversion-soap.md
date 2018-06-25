---
title: RequestedServerVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: cf3f9d7a-2add-4457-b009-2929220f90b5
description: O elemento RequestedServerVersion Especifica a versão do servidor que um método de descoberta automática alvos de chamadas.
ms.openlocfilehash: 6b9d31f3b7bca087652f04e4943becc5ac4e68e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825132"
---
# <a name="requestedserverversion-soap"></a>RequestedServerVersion (SOAP)

O elemento **RequestedServerVersion** Especifica a versão do servidor que um método de **descoberta automática** alvos de chamadas. 
  
```XML
<RequestedServerVersion/>
```

 **ExchangeVersion**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **RequestedServerVersion** Especifica a versão do servidor que um método de **descoberta automática** alvos de chamadas. A tabela a seguir lista as versões de servidor válido. 
  
|**Valor de texto**|**Descrição**|
|:-----|:-----|
|Exchange2007_SP1  <br/> |Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|Exchange2010  <br/> |Exchange Server 2010.  <br/> |
|Exchange2010_SP1  <br/> |Exchange Server 2010 Service Pack 1 (SP1).  <br/> |
|Exchange2010_SP2  <br/> |Exchange Server 2010 Service Pack 2 (SP2).  <br/> |
|Exchange2013  <br/> |Exchange Server 2013. O campo Exchange2013 é aplicável para clientes que visam o Exchange Online e versões do Exchange, começando com o Exchange Server 2013.  <br/> |
|Exchange2013_SP1  <br/> |Exchange Server 2013 Service Pack 1 (SP1). O campo Exchange2013_SP1 é aplicável para clientes que visam o Exchange Online e versões do Exchange, começando com o Exchange Server 2013 SP1.  <br/> |
   
## <a name="remarks"></a>Comentários

O elemento **RequestedServerVersion** é definido no cabeçalho SOAP. 
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   

