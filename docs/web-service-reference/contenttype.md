---
title: ContentType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ContentType
api_type:
- schema
ms.assetid: f91ff0df-0d8a-43ea-a188-d80f0e885f19
description: O elemento ContentType descreve o tipo mime (Extensões de Email da Internet) multiuso do conteúdo de anexo.
ms.openlocfilehash: 3f00aaa2f3b93ab7a8a3ccc4905b1353dce6b083
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526648"
---
# <a name="contenttype"></a>ContentType

O **elemento ContentType** descreve o tipo mime (Extensões de Email da Internet) multiuso do conteúdo de anexo. 
  
```xml
<ContentType/>
```

 **String**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemAttachment](itemattachment.md) <br/> |Representa um Exchange que está anexado a outro Exchange item.  <br/> |
|[FileAttachment](fileattachment.md) <br/> |Representa um arquivo anexado a um item no Exchange store.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto é um valor de cadeia de caracteres que representa o tipo de conteúdo do anexo.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

