---
title: DirectoryPort (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: ab436b54-ceba-4cd9-aeb4-134f9b93986d
description: O elemento DirectoryPort especifica a porta usada para se conectar ao diretório quando o protocolo NSPI (Name Service Provider Interface) é usado.
ms.openlocfilehash: 223e82840628e19896bde196d7467622a2ad5002
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543328"
---
# <a name="directoryport-pox"></a>DirectoryPort (POX)

O **elemento DirectoryPort** especifica a porta usada para se conectar ao diretório quando o protocolo NSPI (Name Service Provider Interface) é usado. 
  
- [AutoDiscover (POX)](autodiscover-pox.md) 
- [Response (POX)](response-pox.md)  
- [Account (POX)](account-pox.md)  
- [Protocol (POX)](protocol-pox.md)  
- [DirectoryPort (POX)](directoryport-pox.md)
  
```xml
<DirectoryPort/>
```

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa a porta usada para acessar o Exchange servidor.
  
## <a name="remarks"></a>Comentários

O **elemento DirectoryPort** só é usado quando o [elemento Type (POX)](type-pox.md) é igual a EXCH ou EXPR. 
  
## <a name="see-also"></a>Confira também

- [Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

