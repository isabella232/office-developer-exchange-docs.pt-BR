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
description: A operação UpdateItem é usada para modificar as propriedades de um item existente no repositório do Exchange.
ms.openlocfilehash: c001b7656862144023e9704cb04e6b4c0030f9df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459388"
---
# <a name="updateitem-operation"></a>Operação UpdateItem

A operação **UpdateItem** é usada para modificar as propriedades de um item existente no repositório do Exchange. 
  
## <a name="remarks"></a>Comentários

Você pode executar três ações básicas de atualização em um item. A tabela a seguir lista as ações que você pode executar.
  
|**Action**|**Descrição**|
|:-----|:-----|
|Append  <br/> |Adiciona dados a uma propriedade existente. Esta ação preserva os dados atuais. Append não se aplica a todas as propriedades.  <br/> |
|Set  <br/> |Substitui dados de uma propriedade se a propriedade contiver dados ou criar a propriedade e define seu valor se a propriedade não existir. A ação Set só é aplicável a propriedades graváveis.  <br/> |
|Excluir  <br/> |Remove uma propriedade de um item. Isso difere da definição de uma propriedade para um valor vazio. Quando essa ação é concluída, a propriedade não existe para o item. Delete só é aplicável a propriedades graváveis.  <br/> |
   
Uma chamada **UpdateItem** pode ser usada para modificar um ou mais itens e uma ou mais propriedades em cada item. O elemento [Mychanges](itemchanges.md) contém todas as modificações que devem ser realizadas como parte desta chamada. O elemento [ItemChange](itemchange.md) , um filho [do elemento items](itemchanges.md) , representa as modificações a serem realizadas em um único item. O elemento [ItemChange](itemchange.md) contém um conjunto de ações de atualização que podem ser executadas em um único item. Essas alterações estão contidas no elemento [Updates (item)](updates-item.md) . O elemento [ItemId](itemid.md) identifica o item a ser atualizado. Para atualizar mais de uma propriedade em um item, um [Setitemfield](setitemfield.md), [AppendToItemField](appendtoitemfield.md)ou [DeleteItemField](deleteitemfield.md) deve ser fornecido para cada propriedade que requer a atualização. 
  
> [!NOTE]
> As ações de atualização são aplicadas na ordem em que são especificadas. 
  
Para cada alteração, você precisa especificar o caminho da propriedade a ser alterada e uma representação desse item com o novo valor. A ação de exclusão é ligeiramente diferente, pois apenas o caminho da propriedade que deve ser excluído é obrigatório. Para ações set e Append, o caminho especificado deve se referir à mesma propriedade que está sendo definida na representação do item. Se forem diferentes, um erro será retornado.
  
A operação **UpdateItem** pode definir a hora de [início](start.md) e de [término](end-ex15websvcsotherref.md) de um item do repositório do Exchange. Em uma solicitação **UpdateItem** , a hora de [início](start.md) pode ser definida sem definir também a hora de [término](end-ex15websvcsotherref.md) . Isso pode causar um erro se a hora de [início](start.md) for posterior à hora de [término](end-ex15websvcsotherref.md) . Lembre-se de que os aplicativos cliente devem ajustar a hora de [término](end-ex15websvcsotherref.md) quando a hora de [início](start.md) é alterada para preservar a duração. 
  
Quando um único item de calendário é atualizado para se tornar um item de calendário mestre recorrente, a propriedade [MeetingTimeZone](meetingtimezone.md) deve ser definida pela operação **UpdateItem** para preservar o fuso horário original do item do calendário. 
  
## <a name="setitemfield-request-example"></a>Exemplo de solicitação setitemfield

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação **UpdateItem** mostra como definir a propriedade sensibilidade em um item. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a>Comentários

O identificador de item e a chave de alteração foram reduzidos para preservar a legibilidade.
  
### <a name="setitemfield-request-elements"></a>Elementos de solicitação setitemfield

Os seguintes elementos são usados na solicitação:
  
- [UpdateItem](updateitem.md)
    
- [Alterações](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [Atualizações (item)](updates-item.md)
    
- [Setitemfield](setitemfield.md)
    
- [FieldURI](fielduri.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [Sensitivity](sensitivity.md)
    
## <a name="appendtoitemfield-request-example"></a>Exemplo de solicitação AppendToItemField

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação **UpdateItem** mostra como acrescentar texto à Propriedade Body em um item. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a>Comentários

As propriedades a seguir dão suporte à ação Append:
  
- **mensagem: ReplyTo**
    
- **item: Body**
    
- Todas as propriedades de coleção Recipient e participante
    
O identificador de item e a chave de alteração foram reduzidos para preservar a legibilidade.
  
### <a name="appendtoitemfield-request-elements"></a>Elementos de solicitação AppendToItemField

Os seguintes elementos são usados na solicitação:
  
- [UpdateItem](updateitem.md)
    
- [Alterações](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [Atualizações (item)](updates-item.md)
    
- [AppendToItemField](appendtoitemfield.md)
    
- [FieldURI](fielduri.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [Body](body.md)
    
## <a name="deleteitemfield-request-example"></a>Exemplo de solicitação DeleteItemField

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação **UpdateItem** mostra como excluir uma propriedade em um item. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a>Comentários

O identificador de item e a chave de alteração foram reduzidos para preservar a legibilidade.
  
### <a name="deleteitemfield-request-elements"></a>Elementos de solicitação DeleteItemField

Os seguintes elementos são usados na solicitação:
  
- [UpdateItem](updateitem.md)
    
- [Alterações](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [Atualizações (item)](updates-item.md)
    
- [DeleteItemField](deleteitemfield.md)
    
- [FieldURI](fielduri.md)
    
## <a name="successful-response-example"></a>Exemplo de resposta bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação **UpdateItem** . 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="664" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <UpdateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a>Comentários

O identificador de item e a chave de alteração foram reduzidos para preservar a legibilidade.
  
### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedidos

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateItemResponse](updateitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateItemResponseMessage](updateitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Itens](items.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [ItemId](itemid.md)
    
## <a name="see-also"></a>Também consulte



[Operação UpdateItem (tarefa)](updateitem-operation-task.md)
  
[Operação UpdateItem (contato)](updateitem-operation-contact.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Atualizando contatos](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[Atualizando tarefas](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

