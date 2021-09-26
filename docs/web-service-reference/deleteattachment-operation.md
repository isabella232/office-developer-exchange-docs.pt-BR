---
title: Operação DeleteAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteAttachment
api_type:
- schema
ms.assetid: 4d48e595-b98c-48e7-bbeb-cacf91d12a78
description: A operação DeleteAttachment é usada para excluir anexos de arquivo e item de um item existente no Exchange store.
ms.openlocfilehash: bd08776e1f4e75204819ef5463e297e3770a34a4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546683"
---
# <a name="deleteattachment-operation"></a>Operação DeleteAttachment

A operação DeleteAttachment é usada para excluir anexos de arquivo e item de um item existente no Exchange store.
  
## <a name="remarks"></a>Comentários

Essa operação permite que você exclua um ou mais anexos por ID.
  
## <a name="deleteattachment-request-example"></a>Exemplo de solicitação DeleteAttachment

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação DeleteAttachment mostra como excluir um anexo de item.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX"/>
      </AttachmentIds>
    </DeleteAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

O identificador de anexo foi reduzido para preservar a capacidade de leitura.
  
### <a name="request-elements"></a>Elementos request

Os seguintes elementos são usados na solicitação:
  
- [DeleteAttachment](deleteattachment.md)
    
- [AttachmentIds](attachmentids.md)
    
- [AttachmentId](attachmentid.md)
    
## <a name="deleteattachment-response-example"></a>Exemplo de resposta DeleteAttachment

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação DeleteAttachment.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <DeleteAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteAttachmentResponseMessage xsi:type="m:DeleteAttachmentResponseMessageType" ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="AAAtAEFkbWluaXN..." RootItemChangeKey="CQAAABYAA..."/>
        </m:DeleteAttachmentResponseMessage>
      </m:ResponseMessages>
    </DeleteAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

A operação CreateAttachment retorna um elemento do tipo AttachmentIdType que inclui **um RootItemId** e **RootItemChangeKey**. Esses atributos não são permitidos para identificadores em uma solicitação DeleteAttachment. DeleteAttachment usa elementos do tipo RequestAttachmentIdType, que não inclui esses atributos.
  
A resposta DeleteAttachment inclui a ID do item pai. Quando os anexos são removidos de um item, a chave de alteração do item é modificada. A nova chave de alteração de item pode ser obtida da resposta DeleteAttachment.
  
> [!NOTE]
> O [identificador RootItemId](rootitemid.md) e ChangeKey foram reduzidos para preservar a capacidade de leitura. 
  
### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedidos

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [DeleteAttachmentResponse](deleteattachmentresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [RootItemId](rootitemid.md)
    
## <a name="see-also"></a>Confira também

- [Operação CreateAttachment](createattachment-operation.md) 
- [Operação GetAttachment](getattachment-operation.md)

