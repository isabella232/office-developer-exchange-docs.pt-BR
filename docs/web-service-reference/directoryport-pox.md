---
title: DirectoryPort (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ab436b54-ceba-4cd9-aeb4-134f9b93986d
description: O elemento DirectoryPort Especifica a porta usada para conectar ao diretório quando o protocolo de Interface de provedor de serviço de nome (NSPI) é usado.
ms.openlocfilehash: 1b73b9cd1d21c73f4e897684371993312f741322
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751819"
---
# <a name="directoryport-pox"></a>DirectoryPort (POX)

O elemento **DirectoryPort** Especifica a porta usada para conectar ao diretório quando o protocolo de Interface de provedor de serviço de nome (NSPI) é usado. 
  
- [Descoberta automática (POX)](autodiscover-pox.md) 
- [Resposta POX)](response-pox.md)  
- [Conta (POX)](account-pox.md)  
- [Protocolo (POX)](protocol-pox.md)  
- [DirectoryPort (POX)](directoryport-pox.md)
  
```xml
<DirectoryPort/>
```

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Protocolo (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa a porta usada para acessar o servidor do Exchange.
  
## <a name="remarks"></a>Comentários

O elemento **DirectoryPort** é usado apenas quando o elemento de [Tipo POX ()](type-pox.md) é igual a EXCH ou EXPR. 
  
## <a name="see-also"></a>Confira também

- [Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

