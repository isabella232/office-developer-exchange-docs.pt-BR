---
title: Operação UpdateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4
description: A operação UpdateItem é usada para modificar as propriedades de um item existente no Exchange store.
ms.openlocfilehash: 6ac09c24c13efff8053fc605ec2c0e6cf2957429
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514057"
---
# <a name="updateitem-operation"></a>Operação UpdateItem

A **operação UpdateItem** é usada para modificar as propriedades de um item existente no Exchange store. 
  
## <a name="remarks"></a>Comentários

Você pode executar três ações básicas de atualização em um item. A tabela a seguir lista as ações que você pode executar.
  
|**Action**|**Descrição**|
|:-----|:-----|
|Append  <br/> |Adiciona dados a uma propriedade existente. Essa ação preserva os dados atuais. Append não se aplica a todas as propriedades.  <br/> |
|Set  <br/> |Substitui os dados de uma propriedade se a propriedade contiver dados ou criar a propriedade e define seu valor se a propriedade não existir. A ação set só é aplicável a propriedades que podem ser escritas.  <br/> |
|Excluir  <br/> |Remove uma propriedade de um item. Isso difere da configuração de uma propriedade para um valor vazio. Quando essa ação é concluída, a propriedade não existe para o item. Delete só é aplicável a propriedades que podem ser escritas.  <br/> |
   
Uma **chamada UpdateItem** pode ser usada para modificar um ou mais itens e uma ou mais propriedades em cada item. O [elemento ItemChanges](itemchanges.md) contém todas as modificações que devem ser executadas como parte dessa chamada. O [elemento ItemChange,](itemchange.md) filho do [elemento ItemChanges,](itemchanges.md) representa as modificações a serem executadas em um único item. O [elemento ItemChange](itemchange.md) contém um conjunto de ações de atualização que podem ser executadas em um único item. Essas alterações estão [contidas no elemento Updates (Item).](updates-item.md) O [elemento ItemId](itemid.md) identifica o item a ser atualizado. Para atualizar mais de uma propriedade em um item, um [SetItemField](setitemfield.md), [AppendToItemField](appendtoitemfield.md)ou [DeleteItemField](deleteitemfield.md) devem ser fornecidos para cada propriedade que exija a atualização. 
  
> [!NOTE]
> As ações de atualização são aplicadas na ordem em que são especificadas. 
  
Para cada alteração, você precisa especificar o caminho da propriedade a ser mudada e uma representação desse item com seu novo valor. A ação de exclusão é ligeiramente diferente porque apenas o caminho da propriedade que deve ser excluído é necessário. Para definir e anexar ações, o caminho especificado deve se referir à mesma propriedade que está sendo definida na representação do item. Se eles diferirem, um erro será retornado.
  
A **operação UpdateItem** pode definir a hora [de início](start.md) [e](end-ex15websvcsotherref.md) término de um Exchange de armazenamento. Em uma **solicitação UpdateItem,** a hora [de](start.md) início pode ser definida sem também definir a [hora de](end-ex15websvcsotherref.md) término. Isso pode causar um erro se a hora [de](start.md) início for posterior à [hora de ](end-ex15websvcsotherref.md) Término. Esteja ciente de que os aplicativos cliente devem ajustar a [hora ](end-ex15websvcsotherref.md) de término quando a hora [de](start.md) início é alterada para preservar a duração. 
  
Quando um único item de calendário é atualizado para se tornar um item de calendário mestre recorrente, a propriedade [MeetingTimeZone](meetingtimezone.md) deve ser definida pela operação **UpdateItem** para preservar o fuso horário original do item de calendário. 
  
## <a name="setitemfield-request-example"></a>Exemplo de solicitação SetItemField

### <a name="description"></a>Descrição

O exemplo a seguir de **uma solicitação UpdateItem** mostra como definir a propriedade de sensibilidade em um item. 
  
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

O identificador de item e a chave de alteração foram reduzidos para preservar a capacidade de leitura.
  
### <a name="setitemfield-request-elements"></a>Elementos de solicitação SetItemField

Os seguintes elementos são usados na solicitação:
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [Updates (Item)](updates-item.md)
    
- [SetItemField](setitemfield.md)
    
- [FieldURI](fielduri.md)
    
- [Mensagem](message-ex15websvcsotherref.md)
    
- [Sensitivity](sensitivity.md)
    
## <a name="appendtoitemfield-request-example"></a>Exemplo de solicitação AppendToItemField

### <a name="description"></a>Descrição

O exemplo a seguir de **uma solicitação UpdateItem** mostra como anexar texto à propriedade body em um item. 
  
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

As seguintes propriedades suportam a ação de anexação:
  
- **message:ReplyTo**
    
- **item:Body**
    
- Todas as propriedades do destinatário e do conjunto de participantes
    
O identificador de item e a chave de alteração foram reduzidos para preservar a capacidade de leitura.
  
### <a name="appendtoitemfield-request-elements"></a>Elementos de solicitação AppendToItemField

Os seguintes elementos são usados na solicitação:
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [Updates (Item)](updates-item.md)
    
- [AppendToItemField](appendtoitemfield.md)
    
- [FieldURI](fielduri.md)
    
- [Mensagem](message-ex15websvcsotherref.md)
    
- [Body](body.md)
    
## <a name="deleteitemfield-request-example"></a>Exemplo de solicitação DeleteItemField

### <a name="description"></a>Descrição

O exemplo a seguir de **uma solicitação UpdateItem** mostra como excluir uma propriedade em um item. 
  
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

O identificador de item e a chave de alteração foram reduzidos para preservar a capacidade de leitura.
  
### <a name="deleteitemfield-request-elements"></a>Elementos de solicitação DeleteItemField

Os seguintes elementos são usados na solicitação:
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [Updates (Item)](updates-item.md)
    
- [DeleteItemField](deleteitemfield.md)
    
- [FieldURI](fielduri.md)
    
## <a name="successful-response-example"></a>Exemplo de resposta bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida a **uma solicitação UpdateItem.** 
  
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

O identificador de item e a chave de alteração foram reduzidos para preservar a capacidade de leitura.
  
### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedidos

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateItemResponse](updateitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateItemResponseMessage](updateitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Itens](items.md)
    
- [Mensagem](message-ex15websvcsotherref.md)
    
- [ItemId](itemid.md)
    
## <a name="see-also"></a>Confira também



[Operação UpdateItem (tarefa)](updateitem-operation-task.md)
  
[Operação UpdateItem (contato)](updateitem-operation-contact.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Atualizando contatos](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[Atualizando tarefas](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

