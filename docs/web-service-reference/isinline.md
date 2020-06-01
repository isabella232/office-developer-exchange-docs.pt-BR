---
title: IsInline
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsInline
api_type:
- schema
ms.assetid: 5e7712c8-372a-4a16-be64-360c5ff3961a
description: O elemento IsInline indica se o anexo aparece embutido em um item.
ms.openlocfilehash: 2b3b6392fe8867ae9782dcb7211c17f4f4d9becd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464207"
---
# <a name="isinline"></a>IsInline

O elemento **IsInline** indica se o anexo aparece embutido em um item. 
  
```xml
<IsInline>true or false</IsInline>
```

 **boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FileAttachment](fileattachment.md) <br/> |Representa um arquivo anexado a um item no repositório do Exchange.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Representa um item do Exchange anexado a outro item do Exchange.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Esse elemento pode ser **true** ou **false**. O valor padrão é **false**.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

