---
title: UnresolvedEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UnresolvedEntry
api_type:
- schema
ms.assetid: 5ac6116a-3b24-40f8-a877-dbe9a6935919
description: O elemento UnresolvedEntry contém o nome de um contato ou lista de distribuição a ser resolvido.
ms.openlocfilehash: 77074d5aed0a799d355fd176a8c9c06f2dffec5a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538664"
---
# <a name="unresolvedentry"></a>UnresolvedEntry

O **elemento UnresolvedEntry** contém o nome de um contato ou lista de distribuição a ser resolvido. 
  
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

O valor do texto representa o nome de um contato público ou lista de distribuição. O comprimento mínimo da cadeia de caracteres é um caractere.
  
## <a name="remarks"></a>Comentários

O valor de texto deste elemento é usado para resolver nomes nos seguintes campos:
  
- Nome
    
- Sobrenome
    
- Nome de exibição
    
- Nome completo
    
- Office
    
- Alias
    
- Endereço SMTP
    
Endereços de email com tipos de roteamento prefixados, como smtp ou sip, são salvos em uma matriz de vários valores. A [operação ResolveNames](resolvenames-operation.md) executa uma combinação parcial com cada valor dessa matriz quando você adiciona o tipo de roteamento no início do nome não resolvido, como "sip:User1@Contoso.com". Se você não especificar um tipo de roteamento, a operação **ResolveNames** será padrão para o tipo de roteamento de smtp, corresponderá a uma propriedade de endereço SMTP principal e não pesquisará a matriz de vários valores. 
  
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

