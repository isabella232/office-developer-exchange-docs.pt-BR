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
description: O elemento RequestedServerVersion especifica a versão do servidor para a qual uma chamada de método de descoberta automática se direciona.
ms.openlocfilehash: ff63c82943bdd3476a4284f5aa2075fc9c0194b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467904"
---
# <a name="requestedserverversion-soap"></a>RequestedServerVersion (SOAP)

O elemento **RequestedServerVersion** especifica a versão do servidor para a qual uma chamada de método de **descoberta automática** se direciona. 
  
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

O valor de texto do elemento **RequestedServerVersion** especifica a versão do servidor de destino de uma chamada de método de **descoberta automática** . A tabela a seguir lista as versões de servidor válidas. 
  
|**Valor de texto**|**Descrição**|
|:-----|:-----|
|Exchange2007_SP1  <br/> |Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|Exchange2010  <br/> |Exchange Server 2010.  <br/> |
|Exchange2010_SP1  <br/> |Exchange Server 2010 Service Pack 1 (SP1).  <br/> |
|Exchange2010_SP2  <br/> |Exchange Server 2010 Service Pack 2 (SP2).  <br/> |
|Exchange2013  <br/> |Exchange Server 2013. O campo Exchange2013 é aplicável para clientes que têm como destino o Exchange Online e versões do Exchange a partir do Exchange Server 2013.  <br/> |
|Exchange2013_SP1  <br/> |Exchange Server 2013 Service Pack 1 (SP1). O campo Exchange2013_SP1 se aplica aos clientes que direcionam o Exchange Online e versões do Exchange a partir do Exchange Server 2013 SP1.  <br/> |
   
## <a name="remarks"></a>Comentários

O elemento **RequestedServerVersion** é definido no cabeçalho SOAP. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |messages. xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   

