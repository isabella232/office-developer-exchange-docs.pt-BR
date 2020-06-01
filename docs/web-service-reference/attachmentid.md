---
title: Attachmentid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentId
api_type:
- schema
ms.assetid: 55a5fd77-60d1-40fa-8144-770600cedc6a
description: O elemento attachmentid identifica um item ou anexo de arquivo. Este elemento é usado em respostas de CreateAttachment.
ms.openlocfilehash: b5dc9299b615f0fc01b8afcbaabf0ec7996e53d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459108"
---
# <a name="attachmentid"></a>Attachmentid

O elemento **attachmentid** identifica um item ou anexo de arquivo. Este elemento é usado em respostas de CreateAttachment. 
  
```xml
<AttachmentId Id="" RootItemId="" RootItemChangeKey="" />
```

 **AttachmentIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Id** <br/> |Identifica o identificador exclusivo do anexo.  <br/> |
|**RootItemId** <br/> |Identifica o identificador exclusivo do item de repositório raiz ao qual o anexo está anexado.  <br/> |
|**RootItemChangeKey** <br/> |Identifica a chave de alteração do item de armazenamento raiz ao qual o anexo está anexado.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemAttachment](itemattachment.md) <br/> |Representa um item do Exchange anexado a outro item do Exchange.  <br/> |
|[FileAttachment](fileattachment.md) <br/> |Representa um arquivo anexado a um item no repositório do Exchange.  <br/> |
   
## <a name="remarks"></a>Comentários

É importante observar que, quando um anexo é criado, a chave de alteração do item raiz é alterada.
  
O elemento [attachmentid (GetAttachment e DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) é usado em solicitações DeleteAttachment e GetAttachment. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

