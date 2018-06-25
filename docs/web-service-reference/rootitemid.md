---
title: RootItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootItemId
api_type:
- schema
ms.assetid: f613c705-17ce-48ce-aa64-4dc2cea25e31
description: O elemento RootItemId identifica o item de raiz de um anexo excluído.
ms.openlocfilehash: 484b185db63c9692eaca7e43c49d6e95375a1a98
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825251"
---
# <a name="rootitemid"></a>RootItemId

O elemento **RootItemId** identifica o item de raiz de um anexo excluído. 
  
[DeleteAttachmentResponse](deleteattachmentresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md)
  
[RootItemId](rootitemid.md)
  
```xml
<RootItemId RootItemId="" RootItemChangeKey="" />
```

 **RootItemIdType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**RootItemId** <br/> |Identifica o item raiz de um anexo excluído.  <br/> |
|**RootItemChangeKey** <br/> |Identifica a nova chave de alteração do item raiz de um anexo excluído.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de DeleteAttachment.  <br/> |
   
## <a name="remarks"></a>Comentários

O elemento **RootItemId** é usado apenas em DeleteAttachment respostas. Isso identifica o identificador de item raiz e mais importante, a nova chave de alteração para o item pai. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[DeleteAttachment](deleteattachment.md)
  
[Operação DeleteAttachment](deleteattachment-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

