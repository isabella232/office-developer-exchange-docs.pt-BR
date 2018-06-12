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
description: O elemento AuthPackage Especifica o esquema de autenticação usado quando se autenticar no servidor do Exchange que possui a função de servidor de caixa de correio instalada.
ms.openlocfilehash: 120ec00ac82166ae2002a8fbac0edf9a1e23afc7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751236"
---
# <a name="authpackage-pox"></a>AuthPackage (POX)

O elemento **AuthPackage** Especifica o esquema de autenticação usado quando se autenticar no servidor do Exchange que possui a função de servidor de caixa de correio instalada. 
  
- [Descoberta automática (POX)](autodiscover-pox.md)
  
- [Resposta POX)](response-pox.md)
  
- [Conta (POX)](account-pox.md)
  
- [Protocolo (POX)](protocol-pox.md)
  
- [AuthPackage (POX)](authpackage-pox.md)
  
```xml
<AuthPackage>basic or kerb or kerbntlm or ntlm or certificate or negotiate or nego2</AuthPackage>
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
|[Protocolo (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente para o servidor de acesso para cliente.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto Especifica o esquema de autenticação que é usado durante a autenticação com base no servidor de caixa de correio. Veja a seguir os valores possíveis:
  
- básico
- KERBTRAY localizado
- kerbntlm
- NTLM
- certificado
- negociar
- nego2
    
## <a name="remarks"></a>Coment�rios

O elemento **AuthPackage** é usado apenas quando o elemento de [Tipo POX ()](type-pox.md) tem um valor de texto de EXCH ou EXPR. 
  
### <a name="version-differences"></a>Diferenças de versão

O Office 365, Exchange Online e versões de local do Exchange começando com compilação 15.00.0995.014 retorno um valor igual a "negociar" somente se o servidor está configurado para usar a autenticação negociar e o cliente incluir um cabeçalho [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) que contém "Negociar". 
  
## <a name="see-also"></a>Confira também

- [Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

