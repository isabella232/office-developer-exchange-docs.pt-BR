---
title: AuthPackage (POX)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 709dbe53-6141-41f8-a2b9-a399bae47991
description: O elemento AuthPackage especifica o esquema de autenticação que é usado na autenticação no servidor do Exchange que tem a função de servidor caixa de Correio instalada.
ms.openlocfilehash: 5317cf49d354a558417829e1d1b5b67cd6874309
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459101"
---
# <a name="authpackage-pox"></a>AuthPackage (POX)

O elemento **AuthPackage** especifica o esquema de autenticação que é usado na autenticação no servidor do Exchange que tem a função de servidor caixa de Correio instalada. 
  
- [Descoberta automática (POX)](autodiscover-pox.md)
  
- [Resposta (POX)](response-pox.md)
  
- [Conta (POX)](account-pox.md)
  
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao servidor de acesso para cliente.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto especifica o esquema de autenticação usado na autenticação no servidor de caixa de correio. Veja a seguir os valores possíveis:
  
- Basic
- kerb
- kerbntlm
- NTML
- certificado
- negocia
- nego2
    
## <a name="remarks"></a>Comentários

O elemento **AuthPackage** é usado somente quando o elemento [tipo (POX)](type-pox.md) tem um valor de texto de Exch ou expr. 
  
### <a name="version-differences"></a>Diferenças de versão

O Office 365, o Exchange Online e as versões locais do Exchange começando com o Build 15.00.0995.014 retornam um valor de "Negotiate" somente se o servidor estiver configurado para usar a autenticação de negociação e o cliente incluir um cabeçalho [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) que contenha "negociar". 
  
## <a name="see-also"></a>Também consulte

- [Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

