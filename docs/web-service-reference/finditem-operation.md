---
title: Operação FindItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- FindItem
api_type:
- schema
ms.assetid: ebad6aae-16e7-44de-ae63-a95b24539729
description: Encontre informações sobre a operação do EWS do FindItem.
localization_priority: Priority
ms.openlocfilehash: 499d1ee80ef323c883fa86eb125d8c037fb37d4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462553"
---
# <a name="finditem-operation"></a>Operação FindItem

Encontre informações sobre a operação do EWS do **FindItem** . 
  
A operação **FindItem** pesquisa itens que estão localizados na caixa de correio de um usuário. Essa operação fornece várias maneiras de filtrar e formatar como os resultados da pesquisa são retornados para o chamador. 
  
## <a name="using-the-finditem-operation"></a>Usando a operação FindItem

A solicitação de operação **FindItem** oferece várias maneiras de Pesquisar uma caixa de correio e formatar como os dados são retornados em uma resposta. Você pode especificar o seguinte em uma solicitação **FindItem** : 
  
- Se a pesquisa é uma passagem superficial ou excluída por software. Especificar isso é necessário. Observe que um percurso excluído por software combinado com uma restrição de pesquisa resultará em zero itens retornados, mesmo se houver itens que correspondam aos critérios de pesquisa.
    
- A forma de resposta dos itens. Isso identifica as propriedades que são retornadas na resposta. Especificar isso é necessário.
    
- As pastas a partir das quais executar a pesquisa. Especificar isso é necessário.
    
- O mecanismo de paginação e os tipos de exibição para retornar dados de modo de exibição em páginas. Especificar isso é opcional.
    
- Opções para agrupar e classificar os itens que são retornados. Especificar isso é opcional.
    
- Restrições de pesquisa ou cadeias de caracteres de sintaxe de consulta avançada (AQS) para filtragem de itens retornados. Para obter mais informações sobre como usar o AQS para pesquisas de índice de conteúdo, consulte [QueryString (cadeia de caracteres)](querystring-string.md). Especificar isso é opcional.
    
- A ordem de classificação de itens retornados na resposta. Especificar isso é opcional.
    
A operação **FindItem** retorna apenas os primeiros 512 bytes de qualquer propriedade streamable. Para Unicode, ele retorna os primeiros 255 caracteres usando uma cadeia de caracteres Unicode terminada em nulo. Ele não retorna nenhum dos formatos de corpo da mensagem nem as listas de destinatários. **FindItem** retornará um resumo de destinatário. Você pode usar a [operação GetItem](getitem-operation.md) para obter os detalhes de um item. 
  
 **FindItem** retorna apenas o elemento [Name (EmailAddressType)](name-emailaddresstype.md) e não retorna o elemento [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) no elemento [Mailbox](mailbox.md) para os seguintes campos: 
  
- O campo [de](from.md) para mensagens 
    
- O campo de [remetente](sender.md) para mensagens 
    
- O campo [organizador](organizer.md) para itens de calendário 
    
> [!NOTE]
> A operação **FindItem** pode retornar resultados em um elemento [CalendarView](calendarview.md) . O elemento **CalendarView** retorna itens de calendário único e todas as ocorrências de reuniões recorrentes. Se um elemento **CalendarView** não for usado, itens de calendário únicos e itens de calendário mestre recorrentes serão retornados. As ocorrências devem ser expandidas do mestre recorrente se um elemento **CalendarView** não for usado. 
  
A operação **FindItem** pode usar os cabeçalhos SOAP listados na tabela a seguir. 
  
**Tabela 1. Cabeçalhos SOAP de operação FindItem**

|**Header**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**DateTimePrecision** <br/> |[DateTimePrecision](datetimeprecision.md) <br/> |Especifica a resolução de valores de data/hora em respostas do servidor, em segundos ou em milissegundos. Isso se aplica a uma solicitação.  <br/> |
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Isso se aplica a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura RFC3066 a ser usada para acessar a caixa de correio. Isso se aplica a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Isso se aplica a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Isso se aplica a uma resposta.  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Identifica o fuso horário a ser usado para todas as respostas do servidor. Isso se aplica a uma solicitação.  <br/> |
   
## <a name="finditem-operation-request-example"></a>Exemplo de solicitação de operação FindItem

O exemplo a seguir de uma solicitação **FindItem** mostra como obter o identificador de item definido pela enumeração **IdOnly** do elemento [BaseShape](baseshape.md) para itens que estão localizados na pasta itens excluídos. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
              Traversal="Shallow">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </ItemShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="deleteditems"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

Os seguintes elementos são usados na solicitação: 
  
- [FindItem](finditem.md)
    
- [Shape](itemshape.md)
    
- [BaseShape](baseshape.md)
    
- [ParentFolderIds](parentfolderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
Para obter mais opções para uma mensagem de solicitação do **FindItem** , explore a hierarquia do esquema. Inicie no elemento [FindItem](finditem.md) . 
  
## <a name="successful-finditem-operation-response"></a>Resposta de operação FindItem bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida à solicitação **FindItem** . 
  
Os elementos da [mensagem](message-ex15websvcsotherref.md) representam mensagens de email e todos os outros itens que não são digitados com rigidez pelo esquema do EWS. Itens como IPM. O compartilhamento e o IPM. InfoPath são retornados como elementos de [mensagem](message-ex15websvcsotherref.md) . O Exchange não retorna o elemento de [Item](item.md) base em respostas. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="10" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AS4AUn=" ChangeKey="fsVU4==" />
              </t:Message>
              <t:Message>
                <t:ItemId Id="AS4AUM=" ChangeKey="fsVUA==" />
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [FindItemResponse](finditemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [FindItemResponseMessage](finditemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md)
    
- [Itens](items.md)
    
- [Mensagem](message-ex15websvcsotherref.md)
    
- [ItemId](itemid.md)
    
Para obter mais opções para uma mensagem de resposta **FindItem** , explore a hierarquia de esquema. Inicie no elemento [FindItemResponse](finditemresponse.md) . 
  
## <a name="finditem-operation-error-response"></a>Resposta de erro de operação FindItem

O exemplo a seguir mostra uma resposta de erro a uma solicitação **FindItem** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

Os seguintes elementos são usados na resposta de erro:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [FindItemResponse](finditemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [FindItemResponseMessage](finditemresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Para obter mais opções para uma mensagem de resposta de erro do **FindItem** , explore a hierarquia de esquema. Inicie no elemento [FindItemResponse](finditemresponse.md) . 
  
## <a name="version-differences"></a>Diferenças de versão

As versões do Exchange que começam com a versão principal 15 e terminando com Build 15.0.898.11 retornam um valor ErrorInvalidOperation no elemento [ResponseCode](responsecode.md) quando a operação **FindItem** é usada para pesquisar várias pastas em uma caixa de correio de arquivo morto. 
  
## <a name="see-also"></a>Confira também

- [Localizar itens](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)
    
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
    
- **FindItemType**
    

