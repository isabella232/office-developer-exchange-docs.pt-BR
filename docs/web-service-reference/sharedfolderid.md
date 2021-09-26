---
title: SharedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SharedFolderId
api_type:
- schema
ms.assetid: 21181ba3-9626-4284-9717-0b1c16948e8f
description: O elemento SharedFolderId representa o identificador da pasta compartilhada para a qual o identificador de pasta local deve ser retornado por uma solicitação de operação GetSharingFolder.
ms.openlocfilehash: 7e47ba49abed99bdb3cfd00eb43d2ef276d4ef37
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545969"
---
# <a name="sharedfolderid"></a>SharedFolderId

O **elemento SharedFolderId** representa o identificador da pasta compartilhada para a qual o identificador de pasta local deve ser retornado por uma solicitação de operação [GetSharingFolder.](getsharingfolder-operation.md) 
  
```xml
<SharedFolderId/>
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
|[GetSharingFolder](getsharingfolder.md) <br/> |Define uma solicitação para obter o identificador de pasta local de uma pasta compartilhada especificada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto é uma cadeia de caracteres que representa o identificador da pasta compartilhada para a qual o identificador de pasta local deve ser retornado por uma solicitação de operação [GetSharingFolder.](getsharingfolder-operation.md) 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetSharingFolder](getsharingfolder-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

