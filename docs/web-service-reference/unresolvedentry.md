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
description: O elemento UnresolvedEntry contém o nome de uma lista de contatos ou de distribuição para resolver.
ms.openlocfilehash: 98b447cd49685b49f73f75f12d921a65749be245
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837860"
---
# <a name="unresolvedentry"></a>UnresolvedEntry

O elemento **UnresolvedEntry** contém o nome de uma lista de contatos ou de distribuição para resolver. 
  
[ResolveNames](resolvenames.md)
  
[UnresolvedEntry](unresolvedentry.md)
  
```xml
<UnresolvedEntry/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResolveNames](resolvenames.md) <br/> |Define uma solicitação para resolver nomes de ambíguos.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa o nome de uma lista de contatos ou de distribuição pública. O comprimento mínimo da cadeia de caracteres é um caractere.
  
## <a name="remarks"></a>Coment�rios

O valor de texto deste elemento é usado para resolver nomes com os seguintes campos:
  
- Nome
    
- Sobrenome
    
- Nome de exibição
    
- Nome completo
    
- Office
    
- Alias
    
- Endereço SMTP
    
Endereços de email com tipos de roteamento de prefixados, como smtp ou sip, são salvas em uma matriz de valores múltiplos. A [operação ResolveNames](resolvenames-operation.md) realiza uma correspondência parcial contra cada valor dessa matriz, quando você adiciona o tipo de roteamento no início do nome não resolvido, como "sip:User1@Contoso.com". Se você não especificar um tipo de roteamento, a operação **ResolveNames** padrão para o tipo de roteamento de smtp, associá-lo a uma propriedade de endereço SMTP principal e não a matriz de vários valores de pesquisa. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação ResolveNames](resolvenames-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

