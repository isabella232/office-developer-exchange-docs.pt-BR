---
title: base64FolderId (serviço web de Unificação de mensagens)
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
description: O elemento base64FolderId contém o identificador da pasta para especificar como a pasta de email padrão do qual Unificação de mensagens lê as mensagens por telefone em uma solicitação do SetTelephoneAccessFolderEmail operação (serviço web de Unificação de mensagens).
ms.openlocfilehash: 7d710542418a717c6fcad243a22682e5840ebbd2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751256"
---
# <a name="base64folderid-um-web-service"></a>base64FolderId (serviço web de Unificação de mensagens)

O elemento **base64FolderId** contém o identificador da pasta para especificar como a pasta de email padrão do qual Unificação de mensagens lê as mensagens por telefone em uma solicitação de [operação SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)](settelephoneaccessfolderemail-operation-um-web-service.md) . 
  
[SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)](settelephoneaccessfolderemail-um-web-service.md)
  
[base64FolderId (serviço web de Unificação de mensagens)](base64folderid-um-web-service.md)
  
```xml
<base64FolderId/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhuma
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)](settelephoneaccessfolderemail-um-web-service.md) <br/> |Define a solicitação para definir a pasta de email de acesso de telefone.  <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. O valor de texto representa a identificação de MAPI da pasta.
  
## <a name="remarks"></a>Comentários

Para definir a pasta de email de acesso de telefone, use a [operação SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)](settelephoneaccessfolderemail-operation-um-web-service.md).
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)](settelephoneaccessfolderemail-um-web-service.md)
  
[Operação de SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)](settelephoneaccessfolderemail-operation-um-web-service.md)
  
[Operação FindFolder](findfolder-operation.md)
  
[Operação FindItem](finditem-operation.md)

