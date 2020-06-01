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
description: O elemento CreateAttachment define uma solicitação para criar um anexo a um item no repositório do Exchange.
ms.openlocfilehash: 4cba1b8865dae5da58b9617b249a29314c67331a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466434"
---
# <a name="createattachment"></a>CreateAttachment

O elemento **CreateAttachment** define uma solicitação para criar um anexo a um item no repositório do Exchange. 
  
```xml
<CreateAttachment>
   <ParentItemId/>
   <Attachments/>
</CreateAttachment>
```

 **CreateAttachmentType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ParentItemId](parentitemid.md) <br/> |Identifica o item do repositório pai do Exchange que contém o anexo criado. O elemento [ParentItemId](parentitemid.md) deve fornecer a ID de um item real do repositório do Exchange. Os itens do repositório real podem ser recuperados usando a [operação GetItem](getitem-operation.md); os anexos são recuperados usando a [operação GetAttachment](getattachment-operation.md). Ocorrerá um erro se [ParentItemId](parentitemid.md) for passado a ID de um anexo de arquivo. Se [ParentItemId](parentitemid.md) representar a ID de um anexo de item existente, a [operação CreateAttachment](createattachment-operation.md) adicionará o novo anexo ao anexo existente.  <br/> Este elemento é necessário para a [operação CreateAttachment](createattachment-operation.md).  <br/> |
|[Anexos](attachments-ex15websvcsotherref.md) <br/> |Contém os itens ou arquivos a serem anexados a um item no repositório do Exchange.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="remarks"></a>Comentários

Um anexo de item não existe como um item de repositório. Ela só existe como um anexo a um item ou outro anexo. Os anexos de item só podem ser recuperados usando a solicitação [GetAttachment](getattachment.md) . 
  
Os seguintes anexos de item podem ser criados:
  
- Item
    
- Mensagem
    
- CalendarItem
    
- Contato
    
- Tarefa
    
- MeetingMessage
    
- MeetingRequest
    
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="example"></a>Exemplo

O exemplo a seguir mostra como criar e anexar um item a outro item no repositório do Exchange.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação CreateAttachment](createattachment-operation.md)
  
[Operação DeleteAttachment](deleteattachment-operation.md)
  
[Operação GetAttachment](getattachment-operation.md)

