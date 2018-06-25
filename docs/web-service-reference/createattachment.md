---
title: CreateAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachment
api_type:
- schema
ms.assetid: e33b403a-b7d3-48ee-8d24-6b7abf0d70bc
description: O elemento de CreateAttachment define uma solicitação para criar um anexo a um item no armazenamento do Exchange.
ms.openlocfilehash: d403eb5ca15623d3a973f7b224dbcde5529cf1bc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751567"
---
# <a name="createattachment"></a>CreateAttachment

O elemento de **CreateAttachment** define uma solicitação para criar um anexo a um item no armazenamento do Exchange. 
  
```xml
<CreateAttachment>
   <ParentItemId/>
   <Attachments/>
</CreateAttachment>
```

 **CreateAttachmentType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ParentItemId](parentitemid.md) <br/> |Identifica o item pai Exchange repositório que contém o anexo criado. O elemento [ParentItemId](parentitemid.md) deve fornecer a identificação de uma troca real armazenam o item. Real de armazenar itens podem ser recuperadas usando a [operação GetItem](getitem-operation.md); anexos serão recuperados usando a [operação GetAttachment](getattachment-operation.md). Ocorrerá um erro se o [ParentItemId](parentitemid.md) é passado a identificação de um anexo de arquivo. Se o [ParentItemId](parentitemid.md) representar a identificação de um anexo de item existente, a [operação CreateAttachment](createattachment-operation.md) adiciona o novo anexo no anexo existente.  <br/> Esse elemento é necessário para a [operação CreateAttachment](createattachment-operation.md).  <br/> |
|[Anexos](attachments-ex15websvcsotherref.md) <br/> |Contém os itens ou arquivos a serem anexados a um item no armazenamento do Exchange.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

Um anexo do item não existe como um item de armazenamento. Ele só existe como um anexo de um item ou outro. Anexos de item só podem ser recuperados usando-se a solicitação [GetAttachment](getattachment.md) . 
  
Os seguintes anexos de item podem ser criados:
  
- Item
    
- Message
    
- CalendarItem
    
- Contato
    
- Tarefa
    
- MeetingMessage
    
- MeetingRequest
    
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="example"></a>Exemplo

O exemplo a seguir mostra como criar e anexar um item a outro item no armazenamento do Exchange.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <ParentItemId Id="ASkAS"/>
      <Attachments>
        <t:ItemAttachment>
          <t:Name>MyAttachment</t:Name>
          <t:Message>
            <t:ItemClass>IPM>Note</t:ItemClass>
            <t:Subject>My attachment subject</t:Subject>
            <t:Body BodyType="Text">My attachment body</t:Body>
          </t:Message>
        </t:ItemAttachment>
      </Attachments>
    </CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação CreateAttachment](createattachment-operation.md)
  
[Operação DeleteAttachment](deleteattachment-operation.md)
  
[Operação GetAttachment](getattachment-operation.md)

