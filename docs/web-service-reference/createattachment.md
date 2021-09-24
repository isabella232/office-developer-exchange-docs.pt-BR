---
title: CreateAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateAttachment
api_type:
- schema
ms.assetid: e33b403a-b7d3-48ee-8d24-6b7abf0d70bc
description: O elemento CreateAttachment define uma solicitação para criar um anexo a um item no Exchange store.
ms.openlocfilehash: 6716a83b0d1ba9d7f39351da60f7009df04a3fa0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515870"
---
# <a name="createattachment"></a>CreateAttachment

O **elemento CreateAttachment** define uma solicitação para criar um anexo a um item no Exchange store. 
  
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
|[ParentItemId](parentitemid.md) <br/> |Identifica o item de armazenamento Exchange pai que contém o anexo criado. O [elemento ParentItemId](parentitemid.md) deve fornecer a ID de um item Exchange store real. Os itens reais do armazenamento podem ser recuperados usando a [operação GetItem;](getitem-operation.md) os anexos são recuperados usando [a operação GetAttachment](getattachment-operation.md). Ocorrerá um erro se [o ParentItemId](parentitemid.md) for passado a ID de um anexo de arquivo. Se [ParentItemId](parentitemid.md) representar a ID de um anexo de item existente, a operação [CreateAttachment](createattachment-operation.md) adiciona o novo anexo ao anexo existente.  <br/> Esse elemento é necessário para a [operação CreateAttachment](createattachment-operation.md).  <br/> |
|[Anexos](attachments-ex15websvcsotherref.md) <br/> |Contém os itens ou arquivos a ser anexados a um item no Exchange store.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

Um anexo de item não existe como um item de loja. Ele só existe como um anexo para um item ou outro anexo. Os anexos de item só podem ser recuperados usando a [solicitação GetAttachment.](getattachment.md) 
  
Os seguintes anexos de item podem ser criados:
  
- Item
    
- Mensagem
    
- CalendarItem
    
- Contact
    
- Tarefa
    
- MeetingMessage
    
- MeetingRequest
    
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="example"></a>Exemplo

O exemplo a seguir mostra como criar e anexar um item a outro item no Exchange store.
  
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

