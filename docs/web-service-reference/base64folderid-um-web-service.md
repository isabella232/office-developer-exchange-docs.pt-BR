---
title: base64FolderId (serviço Web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- base64FolderId
api_type:
- schema
ms.assetid: 662f8f2f-49a7-4c7a-9065-98a02a49cfcd
description: O elemento base64FolderId contém o identificador da pasta a ser especificada como a pasta de email padrão da qual a Unificação de Mensagens lê mensagens pelo telefone em uma solicitação de operação SetTelephoneAccessFolderEmail (serviço Web da UM).
ms.openlocfilehash: 149ad55d0ab09f57b0dc3ace7eb0e17c96265e3f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518929"
---
# <a name="base64folderid-um-web-service"></a>base64FolderId (serviço Web de Unificação de mensagens)

O **elemento base64FolderId** contém o identificador da pasta a ser especificada como a pasta de email padrão da qual a Unificação de Mensagens lê mensagens pelo telefone em uma solicitação de operação [SetTelephoneAccessFolderEmail (serviço Web](settelephoneaccessfolderemail-operation-um-web-service.md) da UM). 
  
[SetTelephoneAccessFolderEmail (serviço Web de Unificação de Mensagens)](settelephoneaccessfolderemail-um-web-service.md)
  
[base64FolderId (serviço Web de Unificação de mensagens)](base64folderid-um-web-service.md)
  
```xml
<base64FolderId/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhuma
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SetTelephoneAccessFolderEmail (serviço Web de Unificação de Mensagens)](settelephoneaccessfolderemail-um-web-service.md) <br/> |Define a solicitação para definir a pasta de email de acesso telefônico.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. O valor de texto representa a ID MAPI da pasta.
  
## <a name="remarks"></a>Comentários

Para definir a pasta de email de acesso telefônico, use a [operação SetTelephoneAccessFolderEmail (serviço Web da UM)](settelephoneaccessfolderemail-operation-um-web-service.md).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[SetTelephoneAccessFolderEmail (serviço Web de Unificação de Mensagens)](settelephoneaccessfolderemail-um-web-service.md)
  
[Operação SetTelephoneAccessFolderEmail (serviço Web de Unificação de Mensagens)](settelephoneaccessfolderemail-operation-um-web-service.md)
  
[Operação FindFolder](findfolder-operation.md)
  
[Operação FindItem](finditem-operation.md)

