---
title: Operação UpdateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4
description: A operação UpdateItem é usada para modificar as propriedades de um item existente no armazenamento do Exchange.
ms.openlocfilehash: 009ba16315017c4418fbd71d49744015c4d6d1b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837913"
---
# <a name="updateitem-operation"></a>Operação UpdateItem

A operação **UpdateItem** é usada para modificar as propriedades de um item existente no armazenamento do Exchange. 
  
## <a name="remarks"></a>Comentários

Você pode executar três ações de atualização básica em um item. A tabela a seguir lista as ações que podem ser executadas.
  
|**Action**|**Descrição**|
|:-----|:-----|
|Acréscimo  <br/> |Adiciona dados a uma propriedade existente. Essa ação preserva os dados atuais. Acrescentar não se aplica a todas as propriedades.  <br/> |
|Conjunto  <br/> |Substitui os dados de uma propriedade se a propriedade contém dados, ou cria a propriedade e define seu valor se a propriedade não existir. A ação set só é aplicável às propriedades graváveis.  <br/> |
|Excluir  <br/> |Remove uma propriedade de um item. Isso é diferente da configuração de uma propriedade para um valor vazio. Quando essa ação for concluída, a propriedade não existe para o item. Excluir só é aplicável às propriedades graváveis.  <br/> |
   
Uma chamada **UpdateItem** pode ser usada para modificar um ou mais itens e uma ou mais propriedades em cada item. O elemento [ItemChanges](itemchanges.md) contém todas as modificações que devem ser executadas como parte desta chamada. O elemento [ItemChange](itemchange.md) , um filho do elemento [ItemChanges](itemchanges.md) , representa as modificações para ser executado em um único item. O elemento de [ItemChange](itemchange.md) contém um conjunto de ações de atualização que podem ser executadas em um único item. Essas alterações estão contidas no elemento [atualizações (Item)](updates-item.md) . O elemento [ItemId](itemid.md) identifica o item a ser atualizado. Para atualizar mais de uma propriedade em um item, um [SetItemField](setitemfield.md), [AppendToItemField](appendtoitemfield.md)ou [DeleteItemField](deleteitemfield.md) deve ser fornecido para cada propriedade que requer a atualização. 
  
> [!NOTE]
> Ações de atualização são aplicadas na ordem na qual foram especificados. 
  
Para cada alteração, você precisará especificar o caminho da propriedade para alterar e uma representação de um item com o seu novo valor. A ação Excluir é ligeiramente diferente apenas o caminho da propriedade que deve ser excluído é necessário. Para definir e acrescentar ações, o caminho especificado deve se referir a mesma propriedade que está sendo definida na representação do item. Se eles forem diferentes, um erro será retornado.
  
A operação **UpdateItem** pode definir a hora de [início](start.md) e [término](end-ex15websvcsotherref.md) de um item de armazenamento do Exchange. Em uma solicitação de **UpdateItem** , a hora de [início](start.md) pode ser definida sem também definir a hora de [término](end-ex15websvcsotherref.md) . Isso pode causar um erro se a hora de [início](start.md) é posterior à hora de [término](end-ex15websvcsotherref.md) . Lembre-se de que os aplicativos cliente devem ajustar a hora de [término](end-ex15websvcsotherref.md) quando a hora de [início](start.md) for alterada para preservar a duração. 
  
Quando um item de calendário único é atualizado para se tornar um item de calendário mestre recorrente, a propriedade [MeetingTimeZone](meetingtimezone.md) deve ser definida pela operação de **UpdateItem** para preservar o fuso horário original do item de calendário. 
  
## <a name="setitemfield-request-example"></a>Exemplo de solicitação de SetItemField

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de **UpdateItem** mostra como definir a propriedade sensitivity em um item. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkb..." ChangeKey="CQAAABYAAAB..."/>
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Sensitivity"/>
              <t:Message>
                <t:Sensitivity>Normal</t:Sensitivity>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comments

O identificador do item e alterar chave foram diminuídas para preservar a legibilidade.
  
### <a name="setitemfield-request-elements"></a>Elementos de solicitação de SetItemField

Os seguintes elementos são usados na solicitação:
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [Atualizações (Item)](updates-item.md)
    
- [SetItemField](setitemfield.md)
    
- [FieldURI](fielduri.md)
    
- [Mensagem](message-ex15websvcsotherref.md)
    
- [Sensitivity](sensitivity.md)
    
## <a name="appendtoitemfield-request-example"></a>Exemplo de solicitação de AppendToItemField

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de **UpdateItem** mostra como acrescentar texto a propriedade body em um item. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkbW..." ChangeKey="CQAAABYA..."/>
          <t:Updates>
            <t:AppendToItemField>
              <t:FieldURI FieldURI="item:Body"/>
              <t:Message>
                <t:Body BodyType="Text">Some additional text to append</t:Body>
              </t:Message>
            </t:AppendToItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comments

As propriedades a seguir oferecem suporte à ação de append:
  
- **mensagem: ReplyTo**
    
- **Corpo do item:**
    
- Todas as participante e destinatário coleção propriedades
    
O identificador do item e alterar chave foram diminuídas para preservar a legibilidade.
  
### <a name="appendtoitemfield-request-elements"></a>Elementos de solicitação de AppendToItemField

Os seguintes elementos são usados na solicitação:
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [Atualizações (Item)](updates-item.md)
    
- [AppendToItemField](appendtoitemfield.md)
    
- [FieldURI](fielduri.md)
    
- [Mensagem](message-ex15websvcsotherref.md)
    
- [Corpo](body.md)
    
## <a name="deleteitemfield-request-example"></a>Exemplo de solicitação de DeleteItemField

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de **UpdateItem** mostra como excluir uma propriedade em um item. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkbWluaXN0cm..." ChangeKey="CQAAABYAA..."/>
          <t:Updates>
            <t:DeleteItemField>
              <t:FieldURI FieldURI="item:Body"/>
            </t:DeleteItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comments

O identificador do item e alterar chave foram diminuídas para preservar a legibilidade.
  
### <a name="deleteitemfield-request-elements"></a>Elementos de solicitação de DeleteItemField

Os seguintes elementos são usados na solicitação:
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [Atualizações (Item)](updates-item.md)
    
- [DeleteItemField](deleteitemfield.md)
    
- [FieldURI](fielduri.md)
    
## <a name="successful-response-example"></a>Exemplo de resposta bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de **UpdateItem** . 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="664" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <UpdateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="AAAtAEFkbW..." ChangeKey="CQAAABYAAA..."/>
            </t:Message>
          </m:Items>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </UpdateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comments

O identificador do item e alterar chave foram diminuídas para preservar a legibilidade.
  
### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedida

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateItemResponse](updateitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateItemResponseMessage](updateitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items](items.md)
    
- [Mensagem](message-ex15websvcsotherref.md)
    
- [ItemId](itemid.md)
    
## <a name="see-also"></a>Confira também



[Operação UpdateItem (tarefa)](updateitem-operation-task.md)
  
[Operação UpdateItem (contato)](updateitem-operation-contact.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Atualizar contatos](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[Atualizar as tarefas](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

