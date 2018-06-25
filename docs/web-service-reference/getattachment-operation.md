---
title: Operação GetAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 24d10a15-b942-415e-9024-a6375708f326
description: A operação GetAttachment é usada para recuperar os anexos existentes em itens no armazenamento do Exchange.
ms.openlocfilehash: c260033208bf49c60463c09041d8ffcc52a8f5c2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752411"
---
# <a name="getattachment-operation"></a>Operação GetAttachment

A operação GetAttachment é usada para recuperar os anexos existentes em itens no armazenamento do Exchange.
  
## <a name="getattachment-request-example"></a>Exemplo de solicitação GetAttachment

### <a name="description"></a>Descrição

O exemplo a seguir de solicitação GetAttachment mostra como obter um anexo.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comments

O elemento [AttachmentShape](attachmentshape.md) permite que você especifique quais informações do anexo devem ser retornadas. Um elemento [AttachmentShape](attachmentshape.md) vazio é válido e será renderizado anexos sem conteúdo MIME para anexos de item, com um tipo de corpo de texto e sem qualquer propriedades adicionais. 
  
A coleção [AttachmentIds](attachmentids.md) permite que você especifique um ou mais identificadores de anexo para retornar. Observe que esses são do tipo RequestAttachmentIdType, portanto, qualquer AttachmentIds recebidos de **CreateAttachment** deve ter os atributos **RootItemId** e **RootItemChangeKey** removido antes de passar os mesmos para **GetAttachment**.
  
> [!NOTE]
> O identificador de anexo e alterar chave foram diminuídas para preservar a legibilidade. 
  
### <a name="request-elements"></a>Elementos de solicitação

Os seguintes elementos são usados na solicitação:
  
- [GetAttachment](getattachment.md)
    
- [AttachmentShape](attachmentshape.md)
    
- [AttachmentIds](attachmentids.md)
    
- [AttachmentId (GetAttachment e DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
## <a name="getattachment-response-example"></a>Exemplo de resposta GetAttachment

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de GetAttachment. Este exemplo retorna um anexo de arquivo.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
              <t:Name>SomeFile</t:Name>
              <t:Content>AQIDBAU=</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </GetAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comments

As mensagens de resposta para GetAttachment sempre conterá o anexo completo; ou seja, todas as propriedades sempre serão incluídas. Anexos de arquivo, essas propriedades são [nome (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md)e [conteúdo](content.md). Anexos de item, essas propriedades são [nome (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) e todas as propriedades do item, como se a forma **AllProperties** tenha sido usada em uma chamada de GetItem. O elemento [AttachmentShape](attachmentshape.md) , se houver, permitirá que um aplicativo de consumidor solicitar as propriedades estendidas adicionais para anexos do item. 
  
### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedida

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetAttachmentResponse](getattachmentresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetAttachmentResponseMessage](getattachmentresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Anexos](attachments-ex15websvcsotherref.md)
    
- [FileAttachment](fileattachment.md)
    
- [AttachmentId (GetAttachment e DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
- [Nome (AttachmentType)](name-attachmenttype.md)
    
- [Conteúdo](content.md)
    
## <a name="see-also"></a>Confira também



[Operação CreateAttachment](createattachment-operation.md)
  
[Operação DeleteAttachment](deleteattachment-operation.md)

