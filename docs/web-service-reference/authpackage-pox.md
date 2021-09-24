---
title: AuthPackage (POX)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 709dbe53-6141-41f8-a2b9-a399bae47991
description: O elemento AuthPackage especifica o esquema de autenticação usado na autenticação no servidor Exchange que tem a função de servidor de Caixa de Correio instalada.
ms.openlocfilehash: aff4e84cd44d76c2c5a913b6627e1b0c87bab4dc
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513021"
---
# <a name="authpackage-pox"></a>AuthPackage (POX)

O **elemento AuthPackage** especifica o esquema de autenticação usado ao autenticar no servidor Exchange que tem a função de servidor de Caixa de Correio instalada. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
  
- [Response (POX)](response-pox.md)
  
- [Account (POX)](account-pox.md)
  
- [Protocol (POX)](protocol-pox.md)
  
- [AuthPackage (POX)](authpackage-pox.md)
  
```xml
<AuthPackage>basic or kerb or kerbntlm or ntlm or certificate or negotiate or nego2</AuthPackage>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao servidor de Acesso para Cliente.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto especifica o esquema de autenticação usado ao autenticar no servidor de Caixa de Correio. Veja a seguir os valores possíveis:
  
- basic
- kerb
- kerbntlm
- ntlm
- certificado
- negociar
- nego2
    
## <a name="remarks"></a>Comentários

O **elemento AuthPackage** só é usado quando o [elemento Type (POX)](type-pox.md) tem um valor de texto de EXCH ou EXPR. 
  
### <a name="version-differences"></a>Diferenças de versão

Office 365, Exchange Online e versões locais do Exchange a partir da com build 15.00.0995.014 retornarão um valor de "negociar" somente se o servidor estiver configurado para usar a autenticação Negociar e o cliente incluir um header [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) que contenha "Negociar". 
  
## <a name="see-also"></a>Confira também

- [Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

