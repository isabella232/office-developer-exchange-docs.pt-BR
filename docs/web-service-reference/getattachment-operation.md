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
description: A operação GetAttachment é usada para recuperar anexos existentes em itens no repositório do Exchange.
ms.openlocfilehash: ac7eafd61c62b077a8d20e5fd8d004924bf06cf1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461286"
---
# <a name="getattachment-operation"></a>Operação GetAttachment

A operação GetAttachment é usada para recuperar anexos existentes em itens no repositório do Exchange.
  
## <a name="getattachment-request-example"></a>Exemplo de solicitação GetAttachment

### <a name="description"></a>Descrição

O exemplo a seguir de solicitação GetAttachment mostra como obter um anexo.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

O elemento [AttachmentShape](attachmentshape.md) permite que você especifique quais informações de anexo devem ser retornadas. Um elemento [AttachmentShape](attachmentshape.md) vazio é válido e renderizará seus anexos sem conteúdo MIME para anexos de item, com um tipo de corpo de texto e sem qualquer outra propriedade. 
  
A coleção [AttachmentIds](attachmentids.md) permite que você especifique um ou mais identificadores de anexo a serem retornados. Observe que eles são do tipo RequestAttachmentIdType, portanto, qualquer AttachmentIds que você receber de **CreateAttachment** deve ter os atributos **RootItemId** e **RootItemChangeKey** removidos antes de passá-los para **GetAttachment**.
  
> [!NOTE]
> O identificador de anexo e a chave de alteração foram reduzidos para preservar a legibilidade. 
  
### <a name="request-elements"></a>Elementos Request

Os seguintes elementos são usados na solicitação:
  
- [GetAttachment](getattachment.md)
    
- [AttachmentShape](attachmentshape.md)
    
- [AttachmentIds](attachmentids.md)
    
- [Attachmentid (GetAttachment e DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
## <a name="getattachment-response-example"></a>Exemplo de resposta de GetAttachment

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação GetAttachment. Este exemplo retorna um anexo de arquivo.
  
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
    <GetAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a>Comentários

As mensagens de resposta para GetAttachment sempre conterão o anexo completo; ou seja, todas as propriedades serão sempre incluídas. Para anexos de arquivo, essas propriedades são [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md)e [Content](content.md). Para anexos de item, essas propriedades são [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) e todas as propriedades do item, como se a forma **myproperties** tivesse sido usada em uma chamada GetItem. O elemento [AttachmentShape](attachmentshape.md) , se presente, permitirá que um aplicativo de consumidor solicite propriedades estendidas adicionais para anexos de item. 
  
### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedidos

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetAttachmentResponse](getattachmentresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetAttachmentResponseMessage](getattachmentresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Anexos](attachments-ex15websvcsotherref.md)
    
- [FileAttachment](fileattachment.md)
    
- [Attachmentid (GetAttachment e DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
- [Nome (AttachmentType)](name-attachmenttype.md)
    
- [Conteúdo](content.md)
    
## <a name="see-also"></a>Também consulte



[Operação CreateAttachment](createattachment-operation.md)
  
[Operação DeleteAttachment](deleteattachment-operation.md)

