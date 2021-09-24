---
title: RequestedServerVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: cf3f9d7a-2add-4457-b009-2929220f90b5
description: O elemento RequestedServerVersion especifica a versão do servidor que um método de Descoberta Automática tem como destino.
ms.openlocfilehash: 0690481523ab48497c40338a8808dfa2ed9b0e99
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540556"
---
# <a name="requestedserverversion-soap"></a>RequestedServerVersion (SOAP)

O **elemento RequestedServerVersion** especifica a versão do servidor que um **método de Descoberta Automática** tem como destino. 
  
```XML
<RequestedServerVersion/>
```

 **ExchangeVersion**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento RequestedServerVersion** especifica a versão do servidor que um **método de Descoberta** Automática direciona. A tabela a seguir lista as versões válidas do servidor. 
  
|**Valor de texto**|**Descrição**|
|:-----|:-----|
|Exchange2007_SP1  <br/> |Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|Exchange2010  <br/> |Exchange Server 2010.  <br/> |
|Exchange2010_SP1  <br/> |Exchange Server 2010 Service Pack 1 (SP1).  <br/> |
|Exchange2010_SP2  <br/> |Exchange Server 2010 Service Pack 2 (SP2).  <br/> |
|Exchange2013  <br/> |Exchange Server 2013. O campo Exchange2013 é aplicável para clientes destinados Exchange Online e versões do Exchange a partir do Exchange Server 2013.  <br/> |
|Exchange2013_SP1  <br/> |Exchange Server 2013 Service Pack 1 (SP1). O campo Exchange2013_SP1 é aplicável para clientes destinados Exchange Online e versões do Exchange a partir do Exchange Server 2013 SP1.  <br/> |
   
## <a name="remarks"></a>Comentários

O **elemento RequestedServerVersion** é definido no header SOAP. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   

