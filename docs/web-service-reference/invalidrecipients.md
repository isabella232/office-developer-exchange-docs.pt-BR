---
title: InvalidRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- InvalidRecipients
api_type:
- schema
ms.assetid: e4e7b50e-2fa9-4649-94a6-6002f341ecc4
description: O elemento InvalidRecipients representa os destinatários de uma solicitação de compartilhamento de pasta inválida.
ms.openlocfilehash: bf9e25b0b0075b99fef8a95b3d4be87727c4cc84
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539539"
---
# <a name="invalidrecipients"></a>InvalidRecipients

O **elemento InvalidRecipients** representa os destinatários de uma solicitação de compartilhamento de pasta inválida. 
  
```XML
<InvalidRecipients>
   <InvalidRecipient/>
</InvalidRecipients>
```

 **ArrayOfInvalidRecipientsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[InvalidRecipient](invalidrecipient.md) <br/> |Contém o endereço SMTP do destinatário inválido e informações sobre por que o destinatário é inválido.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |Define uma resposta a uma [solicitação de operação GetSharingMetadata.](getsharingmetadata-operation.md)  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de operação [GetSharingMetadata.](getsharingmetadata-operation.md)  <br/> |
   
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



[Operação GetSharingMetadata](getsharingmetadata-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

