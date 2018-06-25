---
title: SharedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharedFolderId
api_type:
- schema
ms.assetid: 21181ba3-9626-4284-9717-0b1c16948e8f
description: O elemento SharedFolderId representa o identificador da pasta compartilhada o identificador de pasta local para o qual deve ser retornado por uma solicitação de operação GetSharingFolder.
ms.openlocfilehash: 6d4e541ef3cae89e413efa8cc5f1beaf651dc4dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825477"
---
# <a name="sharedfolderid"></a>SharedFolderId

O elemento **SharedFolderId** representa o identificador da pasta compartilhada o identificador de pasta local para o qual deve ser retornado por uma solicitação de [operação GetSharingFolder](getsharingfolder-operation.md) . 
  
```xml
<SharedFolderId/>
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
|[GetSharingFolder](getsharingfolder.md) <br/> |Define uma solicitação para obter o identificador de pasta local de uma pasta compartilhada especificada.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto é uma cadeia de caracteres que representa o identificador da pasta compartilhada o identificador de pasta local para o qual deve ser retornado por uma solicitação de [operação GetSharingFolder](getsharingfolder-operation.md) . 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação GetSharingFolder](getsharingfolder-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

