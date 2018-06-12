---
title: Operação FindItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItem
api_type:
- schema
ms.assetid: ebad6aae-16e7-44de-ae63-a95b24539729
description: Encontre informações sobre o EWS FindItem operação.
ms.openlocfilehash: b033ac2930981819a20f1336d40058a5f7c03b89
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752289"
---
# <a name="finditem-operation"></a>Operação FindItem

Encontre informações sobre a operação de EWS **FindItem** . 
  
A operação **FindItem** procura itens que estão localizados na caixa de correio do usuário. Esta operação fornece várias maneiras para filtrar e formato como os resultados da pesquisa são retornados ao chamador. 
  
## <a name="using-the-finditem-operation"></a>Usando a operação FindItem

A solicitação de operação **FindItem** oferece diversas maneiras para pesquisar uma caixa de correio e o formato como os dados são retornados em uma resposta. Você pode especificar o seguinte em uma solicitação de **FindItem** : 
  
- Se a pesquisa é uma passagem superficial ou excluída. É necessário especificar isso. Observe que uma passagem excluída combinada com uma restrição de pesquisa resultará em zero itens retornados, mesmo se houver itens que correspondam aos critérios de pesquisa.
    
- A forma de resposta de itens. Isso identifica as propriedades que são retornadas na resposta. É necessário especificar isso.
    
- As pastas do qual efetuar a pesquisa. É necessário especificar isso.
    
- Os tipos de mecanismo e modo de exibição de paginação para retornar exibir dados nas páginas. Especificar isso é opcional.
    
- Opções para agrupar e classificar os itens que são retornados. Especificar isso é opcional.
    
- Restrições de pesquisa ou cadeias de caracteres de sintaxe de consulta avançada (AQS) para filtrar os itens que são retornados. Para obter mais informações sobre como usar o AQS para pesquisas de índice de conteúdo, consulte [QueryString (String)](querystring-string.md). Especificar isso é opcional.
    
- A ordem de classificação para os itens retornados na resposta. Especificar isso é opcional.
    
A operação **FindItem** retorna apenas os primeiros 512 bytes de qualquer propriedade transmissíveis. Para Unicode, ele retorna os primeiros 255 caracteres, usando uma cadeia de caracteres Unicode terminada em nulo. Ele não retorna qualquer um dos formatos de corpo de mensagem ou as listas de destinatário. **FindItem** retornará um destinatário resumo. Você pode usar a [operação GetItem](getitem-operation.md) para obter os detalhes de um item. 
  
 **FindItem** retorna somente o elemento de [nome (EmailAddressType)](name-emailaddresstype.md) e não retorna o elemento [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) no elemento de [caixa de correio](mailbox.md) para os seguintes campos: 
  
- Campo [de](from.md) mensagens 
    
- Campo de [destinatário](sender.md) para mensagens 
    
- O campo [Organizador](organizer.md) para itens de calendário 
    
> [!NOTE]
> A operação **FindItem** pode retornar resultados em um elemento de [exibição de calendário](calendarview.md) . O elemento **CalendarView** retorna todas as ocorrências de reuniões recorrentes e de itens de calendário único. Se um elemento de **exibição de calendário** não for usado, itens de calendário único e itens de calendário mestre recorrentes são retornadas. Se um elemento de **exibição de calendário** não for usado, as ocorrências devem ser expandidas do mestre recorrente. 
  
A operação **FindItem** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir. 
  
**Tabela 1. Cabeçalhos SOAP FindItem operação**

|**Header**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**DateTimePrecision** <br/> |[DateTimePrecision](datetimeprecision.md) <br/> |Especifica a resolução dos valores de data/hora nas respostas do servidor, em segundos ou em milissegundos. Isso é aplicável a uma solicitação.  <br/> |
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Isso é aplicável a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura RFC3066 a ser usado para acessar a caixa de correio. Isso é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Isso é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Isso é aplicável a uma resposta.  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Identifica o fuso horário a ser usado para todas as respostas do servidor. Isso é aplicável a uma solicitação.  <br/> |
   
## <a name="finditem-operation-request-example"></a>Exemplo de solicitação de operação FindItem

O exemplo a seguir de uma solicitação de **FindItem** mostra como obter o identificador do item que é definido pela enumeração **IdOnly** do elemento [BaseShape](baseshape.md) para itens que estão localizados na pasta Itens excluídos. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
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
    
- [ItemShape](itemshape.md)
    
- [BaseShape](baseshape.md)
    
- [ParentFolderIds](parentfolderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
Para obter mais opções para uma mensagem de solicitação **FindItem** , explore a hierarquia de esquema. Inicie o elemento [FindItem](finditem.md) . 
  
## <a name="successful-finditem-operation-response"></a>Resposta de operação FindItem bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida à solicitação **FindItem** . 
  
Elementos de [mensagem](message-ex15websvcsotherref.md) representam as mensagens de email e outros itens que não são fortemente tipados pelo esquema do EWS. Itens como IPM. Compartilhamento e IPM.InfoPath são retornados como elementos da [mensagem](message-ex15websvcsotherref.md) . Exchange não retorna o elemento do [Item](item.md) base nas respostas. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
    
- [Items](items.md)
    
- [Mensagem](message-ex15websvcsotherref.md)
    
- [ItemId](itemid.md)
    
Para obter mais opções para uma mensagem de resposta **FindItem** , explore a hierarquia de esquema. Inicie o elemento [FindItemResponse](finditemresponse.md) . 
  
## <a name="finditem-operation-error-response"></a>Resposta de erro de operação FindItem

O exemplo a seguir mostra uma resposta de erro a uma solicitação de **FindItem** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
    
Para obter mais opções para uma mensagem de resposta de erro **FindItem** , explore a hierarquia de esquema. Inicie o elemento [FindItemResponse](finditemresponse.md) . 
  
## <a name="version-differences"></a>Diferenças de versão

Versões do Exchange, começando com a versão principal 15 e terminando com compilação 15.0.898.11 retornar um valor de ErrorInvalidOperation no elemento [ResponseCode](responsecode.md) quando a operação **FindItem** é usada para pesquisar várias pastas em uma caixa de correio de arquivo morto. 
  
## <a name="see-also"></a>Confira também

- [Localizando itens](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)
    
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
    
- **FindItemType**
    

