---
title: UnresolvedEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnresolvedEntry
api_type:
- schema
ms.assetid: 5ac6116a-3b24-40f8-a877-dbe9a6935919
description: O elemento UnresolvedEntry contém o nome de um contato ou de uma lista de distribuição a ser resolvida.
ms.openlocfilehash: 0f157c1be6c327187456a795c4c1000b8c35b620
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459837"
---
# <a name="unresolvedentry"></a>UnresolvedEntry

O elemento **UnresolvedEntry** contém o nome de um contato ou de uma lista de distribuição a ser resolvida. 
  
[ResolveNames](resolvenames.md)
  
[UnresolvedEntry](unresolvedentry.md)
  
```xml
<UnresolvedEntry/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResolveNames](resolvenames.md) <br/> |Define uma solicitação para resolver nomes ambíguos.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o nome de um contato público ou de uma lista de distribuição. O comprimento mínimo da cadeia de caracteres é um caractere.
  
## <a name="remarks"></a>Comentários

O valor de texto desse elemento é usado para resolver nomes nos seguintes campos:
  
- Nome
    
- Sobrenome
    
- Nome diferenciado (DN)
    
- Nome completo
    
- Office
    
- Alias
    
- Endereço SMTP
    
Os endereços de email com tipos de roteamento prefixos, como SMTP ou SIP, são salvos em uma matriz de vários valores. A [operação ResolveNames](resolvenames-operation.md) executa uma correspondência parcial em relação a cada valor dessa matriz quando você adiciona o tipo de roteamento no início do nome não resolvido, como "SIP:User1@Contoso.com". Se você não especificar um tipo de roteamento, a operação **ResolveNames** usará como padrão o tipo de roteamento do SMTP, o corresponderá a uma propriedade de endereço SMTP primária e não pesquisará a matriz de vários valores. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação ResolveNames](resolvenames-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

