---
title: Identificadores EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 39b6b20b-e081-4347-9e15-9b8cf829fdf0
description: Saiba mais sobre os identificadores no Exchange e como você pode usá-los em seus aplicativos de API gerenciada do EWS e EWS.
localization_priority: Priority
ms.openlocfilehash: 9fa2e31a3c67b0b4291b1e3f32a775655e2bf80a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528423"
---
# <a name="ews-identifiers-in-exchange"></a>Identificadores EWS no Exchange

Saiba mais sobre os identificadores no Exchange e como você pode usá-los em seus aplicativos de API gerenciada do EWS e EWS.
  
Cada objeto no armazenamento do Exchange tem um identificador exclusivo. Você pode usar um identificador de objeto para fazer referência ao objeto e distingui-lo de outros objetos. Os dois identificadores mais comuns que você pode trabalhar são os identificadores de pasta e de item. 
  
Para entender os identificadores e como eles são importantes para seu aplicativo, é útil entender a relação entre objetos no Exchange. Quando a API gerenciada do EWS ou o aplicativo EWS se comunica com o Exchange, você trabalha com uma hierarquia de objetos que inclui os objetos de caixa de correio, pasta e item. Um repositório pode ser qualquer um desses tipos de objeto. Normalmente, é uma caixa de correio no servidor Exchange, mas também pode ser uma pasta pública no servidor Exchange. (Lembre-se de que no Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange a partir do Exchange 2013, as pastas públicas são apenas outro tipo de caixa de correio e não um tipo diferente de armazenamento.) O repositório contém pastas e as pastas contêm itens, e cada uma dessas pastas e itens tem um identificador, conforme mostrado na figura a seguir. 
  
**Figura 1. Hierarquia de caixa de correio, pasta e item**

![Uma ilustração que mostra a hierarquia de objetos da caixa de correio. A caixa de correio está no nível superior com a pasta Caixa de Entrada no nível seguinte. O diagrama mostra uma pasta que contém emails. Identificadores e teclas de alteração são listados para cada objeto e encurtados.](media/Ex15_Identifier_diagram.png)
  
## <a name="ews-identifiers"></a>Identificadores do EWS
<a name="bk_CommonIdentifiers"> </a>

Os identificadores que o EWS usa para pastas e itens são chamados de identificadores EWS ou EwsIds. O EwsIds pode ser encontrado em vários objetos diferentes no EWS, mas é chamado de algo diferente para diferentes objetos. Como você pode usar esses objetos em seu aplicativo, convém entender como os identificadores desses objetos se relacionam com o EwsId. 
  
Os identificadores no EWS também se aplicam à API gerenciada do EWS. Na API gerenciada do EWS, os identificadores são propriedades dos objetos e são gerenciados internamente para mapear para os elementos do EWS.
  
**Tabela 1. Identificadores de objeto no EWS**

|**Object**|**Identificador**|**Como ele se relaciona com o EwsId?**|
|:-----|:-----|:-----|
|[CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |O elemento filho [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) contém o identificador exclusivo do item do calendário.  <br/> |O elemento filho [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) é o mesmo que o EwsId para esse item.  <br/> |
|[ConversationId](https://msdn.microsoft.com/library/d5f1ddb3-9af3-4677-a6ba-111b304a951e%28Office.15%29.aspx) <br/> |O atributo **ID** contém o identificador da conversa que este item faz parte.  <br/> |O atributo **ID** é o mesmo que o EwsId para esse item.  <br/> |
|[Attachmentid](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) <br/> |Fornece o identificador exclusivo do anexo. O atributo [RootItemId](https://msdn.microsoft.com/library/f613c705-17ce-48ce-aa64-4dc2cea25e31%28Office.15%29.aspx) contém o identificador exclusivo do item de repositório raiz ao qual o anexo está anexado.  <br/> |Os anexos podem ser outros itens no repositório do Exchange, caso em que [attachmentid](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) é o mesmo que o EwsId. Em todos os casos, [RootItemId](https://msdn.microsoft.com/library/f613c705-17ce-48ce-aa64-4dc2cea25e31%28Office.15%29.aspx) é um EwsId, pois faz referência a um item no repositório.  <br/> |
|[Personaid](https://msdn.microsoft.com/library/eec3a468-afd5-4d72-a61e-cd1964fb686c%28Office.15%29.aspx) <br/> |O atributo **ID** retorna uma cadeia de caracteres que contém o identificador da pessoa.  <br/> |O atributo **ID** é o mesmo que o EwsId para o persona.  <br/> |
|[ContactID](https://msdn.microsoft.com/library/86f66275-1e39-48ed-bd89-ac3bffc465a7%28Office.15%29.aspx) <br/> |O atributo **ID** retorna uma cadeia de caracteres que contém o identificador do contato.  <br/> |O atributo **ID** é o mesmo que o EwsId para o contato.  <br/> |
|[GroupId](https://msdn.microsoft.com/library/656d9b9a-8a65-4a75-8466-5b0d96512dab%28Office.15%29.aspx) <br/> |O atributo **ID** retorna uma cadeia de caracteres que contém o identificador do grupo.  <br/> |O atributo **ID** é o mesmo que o EwsId para o grupo.  <br/> |
|[AssociatedCalendarItemId](https://msdn.microsoft.com/library/5b29898c-ea59-4e6a-914c-c011ec754032%28Office.15%29.aspx) <br/> |O atributo **ID** identifica o item de calendário associado a um [MeetingMessage](https://msdn.microsoft.com/library/c95956a8-7505-44b4-bea4-11d1f5182796%28Office.15%29.aspx), [MeetingRequest](https://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx), [MeetingResponse](https://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx)ou [MeetingCancellation](https://msdn.microsoft.com/library/a9c61f7f-2ecd-4b21-9dce-24d9f61aeeea%28Office.15%29.aspx).  <br/> |O atributo **ID** é o mesmo que o EwsId para o item do calendário.  <br/> |
|[Userconfigurationproperties](https://msdn.microsoft.com/library/c143a6ec-62ad-4d48-b844-b1ad88054bc1%28Office.15%29.aspx) <br/> |O valor de **ID** desse elemento Especifica a propriedade Identifier.  <br/> |Esse identificador não é mapeado diretamente para o EwsId desde que ele seja um identificador de propriedade e não um item.  <br/> |
|[OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) <br/> |O atributo **recurringMasterId** identifica o mestre de um item recorrente.  <br/> |O valor **OccurrenceItemId** não é mapeado diretamente para o EwsId, mas o **recurringMasterId** faz referência ao objeto de nível superior do item recorrente.  <br/> |
|[StoreEntryId](https://msdn.microsoft.com/library/f536e264-8c4d-4cc5-bab8-22a4fa38de39%28Office.15%29.aspx) <br/> |Contém o identificador de repositório do Exchange de um item.  <br/> |O valor **StoreEntryId** não é mapeado para o EwsId, mas fornece o identificador do repositório em que os itens são mantidos.  <br/> |
   
## <a name="working-with-identifiers"></a>Trabalhar com identificadores
<a name="bk_WorkingWithIdentifiers"> </a>

O servidor do Exchange manipula identificadores de várias maneiras diferentes. Considere o seguinte ao desenvolver sua API gerenciada do EWS ou aplicativo do EWS:
  
- O valor do elemento **ItemId** para pastas e itens diferencia maiúsculas de minúsculas. Se você examinar a ID de item de uma pasta ou item retornado pela [operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) (ou o método de API gerenciada do EWS do [FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ), poderá achar que é uma duplicata de outra ID de item; no entanto, um ou mais caracteres nas IDs de item para os dois itens terão um caso diferente. 
    
- Se você for armazenar a ID do item em um banco de dados para recuperar mais tarde, recomendamos que o tamanho do campo seja 512 bytes, para que seja grande o suficiente para conter o GUID.
    
- Não presuma que a ID do item será sempre válida se você precisar recuperar o item mais tarde. Se um item for movido no repositório, a ID poderá ser alterada devido à forma como uma movimentação é manipulada. Um item é realmente copiado, e um novo ID é gerado e, em seguida, [o item original é excluído](deleting-items-by-using-ews-in-exchange.md). Observe que as IDs de pasta são imutáveis e não serão alteradas quando movidas no repositório.
    
- Os identificadores no Exchange são opacos. Por exemplo, o EwsId é criado de várias partes de informações que não são importantes para você como desenvolvedor, mas são importantes para o Exchange.
    
- Ao trabalhar com itens no Exchange, outro valor para ter em mente é o atributo **ChangeKey** . Esse valor, além da ID do item, é usado para acompanhar o estado de um item. Sempre que um item é alterado, uma nova chave de alteração é gerada. Ao executar uma [operação UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx), por exemplo, você pode usar o atributo **ChangeKey** para permitir que o servidor saiba que a atualização está sendo aplicada à versão mais recente do item. Se outro aplicativo fez uma alteração no item que você está atualizando, as chaves de alteração não serão correspondentes e você não poderá executar a atualização. 
    
## <a name="distinguished-folder-ids"></a>IDs de pastas diferenciadas
<a name="bk_DistinguishedFolderIds"> </a>

O Exchange inclui um número de pastas de caixa de correio predefinidas, cada uma atribuída a um identificador, conhecido como ID de pasta distinta. Eles são definidos pela enumeração API gerenciada do EWS [WellKnownFolderName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) e o elemento EWS [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) . Você pode usar essas IDs de pasta distinta para fazer referência a mais facilmente uma das pastas predefinidas. Por exemplo, para a pasta caixa de entrada, você pode simplesmente usar "caixa de entrada" para o identificador, em vez de determinar o identificador de pasta. 
  
Outras pastas que você cria para organizar itens de email também têm uma ID exclusiva para essa pasta. Essa ID não é alterada mesmo se você alterar outras propriedades na pasta.
  
Você pode usar IDs de pastas diferenciadas como ponto de entrada para acesso de representante. Ao iniciar o acesso de representante, você pesquisa itens ou pastas e fornece a ID de pasta distinta para especificar onde Pesquisar. Quando um usuário representante acessa o servidor, um elemento de [caixa de correio](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) que é filho do elemento **DistinguishedFolderId** é usado para especificar explicitamente a caixa de correio para o representante acessar. 
  
## <a name="handling-errors"></a>Tratamento de erros
<a name="bk_DealingWithErrors"> </a>

Todos os programas estão vinculados para obter um erro a cada momento e, em seguida, e os aplicativos baseados no EWS não são exceção (pun). Você pode receber alguns erros relacionados ao identificador no elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) do EWS ou como parte da enumeração da API gerenciada do EWS do [erro](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) . 
  
Os seguintes erros podem ocorrer na API gerenciada do EWS ou no aplicativo EWS. Se você estiver trabalhando com um aplicativo de API gerenciada por EWS, os erros normalmente são problemas com valores de propriedade; para aplicativos EWS, os erros são associados a valores de elemento XML ou operações.
  
**Tabela 2. Erros relacionados a identificadores**

|**Error**|**Ocorre quando...**|**Descrição**|
|:-----|:-----|:-----|
|ErrorCalendarCannotUseIdForOccurrenceId  <br/> |O valor do **OccurenceID** não corresponde a um item de calendário recorrente válido.  <br/> |O valor do **OccurenceId** especificado na solicitação pode ser válido na estrutura, mas a solicitação não pôde ser correspondente a um mestre recorrente existente. O item recorrente pode ser removido do calendário. Verifique se o item ainda existe e se você está usando o identificador correto.  <br/> |
|ErrorCalendarCannotUseIdForRecurringMasterId  <br/> |O atributo **recurringMasterId** não corresponde a uma ocorrência válida do elemento **Occurrences** .  <br/> |O valor do **recurringMasterId** especificado na solicitação pode ser válido na estrutura, mas a solicitação não pôde ser correspondente a uma ocorrência existente do item. A ocorrência do item pode ser removida do calendário. Verifique se o item ainda existe e se você está usando o identificador correto.  <br/> |
|ErrorCannotUseFolderIdForItemId  <br/> |A **ID** que foi passada representa uma pasta em vez de um item.  <br/> |O identificador pode ser válido no formato, mas não o que o servidor estava esperando para a operação. Verifique se você está fazendo referência ao identificador correto para a operação.  <br/> |
|ErrorCannotUseItemIdForFolderId  <br/> |A **ID** passada representa um item em vez de uma pasta.  <br/> |O identificador pode ser válido no formato, mas não o que o servidor estava esperando para a operação. Verifique se você está fazendo referência à **ID** correta para a operação.  <br/> |
|ErrorChangeKeyRequiredForWriteOperations  <br/> |Uma chave de alteração válida deve ser fornecida quando você estiver realizando determinadas operações de atualização.  <br/> |Você pode omitir um valor de **ChangeKey** quando solicitou uma atualização ou a chave de alteração estava incorreta. Verifique se você tem a chave de alteração correta ao executar operações de atualização.  <br/> |
|ErrorInvalidAttachmentId  <br/> |O anexo não foi encontrado dentro da coleção Attachments do item.  <br/> |Você pode receber esse código de resposta se tiver uma **ID** de anexo e o anexo for excluído e você tentar chamar a [operação GetAttachment](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) na ID de anexo. Verifique se o anexo existe na coleção de anexos.  <br/> |
|ErrorInvalidChangeKey  <br/> |Uma chave de alteração inválida foi passada.  <br/> |Observe que muitas operações e métodos não exigem que uma chave de alteração seja passada. No entanto, se você fornecer uma chave de alteração, ela deve ser válida, embora não precise necessariamente estar atualizada.  <br/> |
|ErrorInvalidFolderId  <br/> |A **ID** da pasta está corrompida.  <br/> |Verifique se você tem um identificador válido e formatado corretamente.  <br/> |
|ErrorInvalidId  <br/> |A estrutura da **ID** e/ou a chave de alteração é internamente inconsistente.  <br/> |O Exchange encontrou um problema com a **ID** após sua análise. Pode ter havido um erro na conversão. Isso pode ocorrer, por exemplo, se você tiver um **idformattype. HexEntryId** para um item no Outlook, mas convertê-lo em um EwsId pensando que era um formato **Idformattype. EntryID** . Certifique-se de usar o tipo de conversão correto.  <br/> |
|ErrorInvalidIdEmpty  <br/> |O aplicativo especificou uma **ID** que está vazia.  <br/> |O aplicativo passou uma cadeia de caracteres vazia para o identificador. Verifique se você tem um identificador válido e formatado corretamente.  <br/> |
|ErrorInvalidIdMalformed  <br/> |A estrutura da **ID** é internamente inconsistente.  <br/> |O Exchange encontrou um problema com a **ID** após sua análise. A ID pode não ter sido convertida corretamente. Certifique-se de usar o tipo de conversão correto.  <br/> |
|ErrorInvalidIdMalformedEwsLegacyIdFormat  <br/> |Uma **ID** de pasta ou de item que está usando o formato Exchange 2007 foi especificada para uma solicitação com uma versão do Exchange 2007 SP1 ou posterior.  <br/> |Você não pode usar IDs do Exchange 2007 no Exchange 2007 SP1 ou em solicitações posteriores. Você deve usar a operação [convertid](https://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx) EWS ou o método de API gerenciada do EWS de [conversão](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.convertid%28v=exchg.80%29.aspx) para convertê-los primeiro.  <br/> |
|ErrorInvalidIdNotAnItemAttachmentId  <br/> |A propriedade **attachmentid** não se refere a um anexo de item.  <br/> |O identificador pode ser válido no formato, mas não o que o servidor estava esperando para a operação. Verifique se você está fazendo referência ao identificador correto para a operação.  <br/> |
|ErrorInvalidIdReturnedByResolveNames  <br/> |Um contato da caixa de correio está corrompido.  <br/> |A operação [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) do EWS ou o método de API gerenciada do EWS de [ResolveName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) retornou um ou mais identificadores, mas eles não são válidos. Talvez seja necessário recriar o contato.  <br/> |
|ErrorInvalidIdStoreObjectIdTooLong  <br/> |A estrutura da **ID** é internamente inconsistente.  <br/> |O Exchange encontrou um problema com a **ID** após sua análise. A **ID** pode não ter sido convertida corretamente. Certifique-se de usar o tipo de conversão correto.  <br/> |
|ErrorInvalidIdTooManyAttachmentLevels  <br/> |As hierarquias de anexos excedem o máximo de 255 níveis de profundidade.  <br/> |O valor da propriedade **attachmentid** que foi especificada na solicitação pode ser válido na estrutura, mas o anexo solicitado é muito profundo na hierarquia. Seu código pode ter tentado anexar um item além do limite de 255 níveis.  <br/> |
|ErrorInvalidImContactId  <br/> |Esse erro pode ser retornado quando o contato não pode ser encontrado no grupo de mensagens instantâneas quando você usa a [operação RemoveImContactFromGroup](https://msdn.microsoft.com/library/a190bbec-c71b-4e6a-880b-55854c724d8c%28Office.15%29.aspx). Este erro se aplica aos clientes que direcionam o Exchange Online e versões do Exchange a partir do Exchange 2013.  <br/> |O valor da propriedade **ContactID** especificada na solicitação pode ser válido na estrutura, mas nenhum contato na caixa de correio corresponde a essa estrutura. Talvez o contato já tenha sido removido.  <br/> |
|ErrorInvalidImGroupId  <br/> |Este erro pode ser retornado quando o grupo não pode ser encontrado na caixa de correio quando você usa a [operação RemoveImGroup](https://msdn.microsoft.com/library/5e788016-68e0-4a3f-9243-03f6b6c6b389%28Office.15%29.aspx). Este erro se aplica aos clientes que direcionam o Exchange Online e versões do Exchange a partir do Exchange 2013.  <br/> |O valor da propriedade **GroupId** especificada na solicitação pode ser válido na estrutura, mas nenhum grupo na caixa de correio corresponde a essa estrutura. O grupo pode ter sido removido.  <br/> |
|ErrorInvalidReferenceItem  <br/> |O identificador do item referenciado não é um **MessageType** ou **ExchangeWebServices. CalendarItemTypeType**ou um de seus descendentes. O identificador do item de referência é para um objeto **CalendarItemType** e o organizador está tentando responder ou ReplyAll.  <br/> |O identificador pode ser válido no formato, mas não o que o servidor estava esperando para a operação. Verifique se você está fazendo referência ao identificador correto para a operação.  <br/> |
|ErrorMissingManagedFolderId  <br/> |A propriedade IDs de política, marca de propriedade 0x6732, para a pasta está ausente.  <br/> |A pasta está corrompida. Considere recriá-lo.  <br/> |
   
## <a name="converting-identifiers"></a>Convertendo identificadores
<a name="bk_ConvertingIdentifiers"> </a>

Talvez seja necessário converter um identificador de um formato para outro. Por exemplo, você pode precisar converter um identificador de um EWS externo, como um identificador que vem de uma conexão MAPI, para um formato que seu aplicativo pode usar. Para fazer isso, você pode usar a operação [convertid](https://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx) do EWS ou o método de API gerenciada do EWS da [conversão](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.convertid%28v=exchg.80%29.aspx) . 
  
Por exemplo, uma EntryID é um identificador exclusivo gerado pelo repositório de mensagens MAPI atribuído pelo repositório quando o item é salvo. Para usar um EntryID em seu aplicativo, primeiro você precisa convertê-lo em um EwsId. 
  
O Outlook Web App usa sua própria versão de identificadores, chamada OwaId, em URLs para acessar pastas e itens. Se seu aplicativo precisar acessar itens no Outlook Web App, você precisará converter o OwaId em um EwsId.
  
Você pode usar a operação **convertid** ou o método para converter vários formatos de identificadores diferentes. 
  
**Tabela 3. Formatos de identificador conversíveis no Exchange**

|**Format**|**Descrição**|
|:-----|:-----|
|EwsLegacyId  <br/> |O EwsId que se aplica ao Exchange 2007.  <br/> |
|EwsId  <br/> |O EwsId que se aplica ao Exchange Online e às versões do Exchange a partir do Exchange 2007 SP1.  <br/> |
|StoreId  <br/> |O identificador do repositório do Exchange onde as pastas e itens são armazenados.  <br/> |
|OwaId  <br/> |O identificador do Outlook Web App usado com o Outlook Web App no Exchange 2007 e no Exchange 2010. <br/><br/>**Observação**: o Exchange Online e versões do Exchange a partir do Exchange 2013 usam o EwsId para Outlook Web App.           |
|EntryId  <br/> |Um identificador MAPI comumente conhecido como a propriedade **PR_ENTRYID** de uma mensagem MAPI.  <br/> |
|HexEntryId  <br/> |Uma representação codificada em hexadecimal da propriedade **PR_ENTRYID** que é usada para o identificador de eventos do calendário de disponibilidade. Este também é o formato de identificador que o Outlook usa.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)  
- [Operação convertid](https://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx)  
- [Enumeração de erro](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) 
- [Excluir itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md)
    

