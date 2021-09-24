---
title: Conteúdo
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Content
api_type:
- schema
ms.assetid: 24f8c54a-505f-4fc0-b7e7-93ad50b97070
description: O elemento Content contém o conteúdo codificado em Base64 de um anexo de arquivo.
ms.openlocfilehash: ccea4412416575f9a1d56a4cde6ebbfd0df31101
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513819"
---
# <a name="content"></a>Conteúdo

O **elemento Content** contém o conteúdo codificado em Base64 de um anexo de arquivo. 
  
```xml
<Content/>
```

 **Base64Binary**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FileAttachment](fileattachment.md) <br/> |Representa um arquivo t que está desconectado a um item no Exchange store.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor da cadeia de caracteres representa os dados binários codificados em Base64 do anexo de arquivo.
  
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

