---
title: base64FolderId (serviço Web da UM)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- base64FolderId
api_type:
- schema
ms.assetid: 662f8f2f-49a7-4c7a-9065-98a02a49cfcd
description: O elemento base64FolderId contém o identificador da pasta para especificar como a pasta de email padrão da qual a Unificação de mensagens lê mensagens por telefone em uma solicitação de operação do SetTelephoneAccessFolderEmail (serviço da Web da UM).
ms.openlocfilehash: ea31c7a0f93188e563bf95c4a3e6e91f0866746c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458044"
---
# <a name="base64folderid-um-web-service"></a>base64FolderId (serviço Web da UM)

O elemento **base64FolderId** contém o identificador da pasta para especificar como a pasta de email padrão da qual a Unificação de mensagens lê mensagens por telefone em uma solicitação de [operação do SetTelephoneAccessFolderEmail (serviço da Web da um)](settelephoneaccessfolderemail-operation-um-web-service.md) . 
  
[SetTelephoneAccessFolderEmail (serviço Web da UM)](settelephoneaccessfolderemail-um-web-service.md)
  
[base64FolderId (serviço Web da UM)](base64folderid-um-web-service.md)
  
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
|[SetTelephoneAccessFolderEmail (serviço Web da UM)](settelephoneaccessfolderemail-um-web-service.md) <br/> |Define a solicitação para definir a pasta de email de acesso telefônico.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é obrigatório. O valor de texto representa a ID de MAPI da pasta.
  
## <a name="remarks"></a>Comentários

Para definir a pasta de email de acesso telefônico, use a [operação SetTelephoneAccessFolderEmail (serviço Web da um)](settelephoneaccessfolderemail-operation-um-web-service.md).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[SetTelephoneAccessFolderEmail (serviço Web da UM)](settelephoneaccessfolderemail-um-web-service.md)
  
[Operação SetTelephoneAccessFolderEmail (serviço Web da UM)](settelephoneaccessfolderemail-operation-um-web-service.md)
  
[Operação FindFolder](findfolder-operation.md)
  
[Operação FindItem](finditem-operation.md)

