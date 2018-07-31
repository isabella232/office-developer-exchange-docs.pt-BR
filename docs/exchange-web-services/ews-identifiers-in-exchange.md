---
title: Identificadores EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 39b6b20b-e081-4347-9e15-9b8cf829fdf0
description: Saiba mais sobre identificadores no Exchange e como você pode usá-los nos seus EWS Managed API e os aplicativos de EWS.
ms.openlocfilehash: fbf6d7756f73b1c5d345f3b34deeb7ea8a347986
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353970"
---
# <a name="ews-identifiers-in-exchange"></a>Identificadores EWS no Exchange

Saiba mais sobre identificadores no Exchange e como você pode usá-los nos seus EWS Managed API e os aplicativos de EWS.
  
Cada objeto no repositório do Exchange tem um identificador exclusivo. Você pode usar um identificador de objeto para fazer referência ao objeto e para diferenciá-lo de outros objetos. Os dois identificadores mais comuns que você pode trabalhar com são pasta e identificadores de item. 
  
Para entender identificadores e como elas são importantes para seu aplicativo, é útil compreender a relação entre os objetos no Exchange. Quando seu aplicativo de EWS ou a API gerenciada de EWS se comunica com o Exchange, você trabalha com uma hierarquia de objetos que inclui a caixa de correio, pasta e objetos de item. Um repositório pode ser qualquer um desses tipos de objeto. Mais comumente, é uma caixa de correio no Exchange server, mas também pode ser uma pasta pública no Exchange server. (Tenha em mente que no Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange, começando com o Exchange 2013, as pastas públicas são qualquer outro tipo de caixa de correio e não um tipo diferente de repositório). O repositório contém pastas e as pastas contêm itens e cada uma dessas pastas e itens tem um identificador, conforme mostrado na figura a seguir. 
  
**Figura 1. Caixa de correio, pasta e hierarquia de item**

![Uma ilustração que mostra a hierarquia de objetos da caixa de correio. A caixa de correio está no nível superior com a pasta Caixa de Entrada no nível seguinte. O diagrama mostra uma pasta que contém emails. Identificadores e teclas de alteração são listados para cada objeto e encurtados.](media/Ex15_Identifier_diagram.png)
  
## <a name="ews-identifiers"></a>Identificadores EWS
<a name="bk_CommonIdentifiers"> </a>

Identificadores que utiliza o EWS para pastas e itens são chamados de identificadores EWS ou EwsIds. EwsIds pode ser encontrado em vários objetos diferentes dentro do EWS, mas são chamados algo diferente para objetos diferentes. Como você pode usar esses objetos em seu aplicativo, você vai querer entender como os identificadores para esses objetos se relacionam a EwsId. 
  
Os identificadores de EWS são aplicáveis para o EWS Managed API também. Na API gerenciada do EWS, os identificadores são propriedades dos objetos em são gerenciados internamente para mapear para os elementos do EWS.
  
**Tabela 1. Identificadores de objeto no EWS**

|**Object**|**Identificador**|**Como ele se relacionam com EwsId?**|
|:-----|:-----|:-----|
|[CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |Elemento filho [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) contém o identificador exclusivo do item de calendário.  <br/> |Elemento filho [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) é igual a EwsId deste item.  <br/> |
|[ConversationId](http://msdn.microsoft.com/library/d5f1ddb3-9af3-4677-a6ba-111b304a951e%28Office.15%29.aspx) <br/> |O atributo **Id** contém o identificador para que esse item é parte da conversa.  <br/> |O atributo **Id** é igual a EwsId deste item.  <br/> |
|[AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) <br/> |Fornece o identificador exclusivo do anexo. O atributo [RootItemId](http://msdn.microsoft.com/library/f613c705-17ce-48ce-aa64-4dc2cea25e31%28Office.15%29.aspx) contém o identificador exclusivo do item raiz repositório à qual o anexo está vinculado.  <br/> |Anexos podem ser outros itens no armazenamento do Exchange, caso em que o [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) será o mesmo que o EwsId. Em todos os casos, o [RootItemId](http://msdn.microsoft.com/library/f613c705-17ce-48ce-aa64-4dc2cea25e31%28Office.15%29.aspx) é um EwsId porque ele faz referência a um item no repositório.  <br/> |
|[PersonaId](http://msdn.microsoft.com/library/eec3a468-afd5-4d72-a61e-cd1964fb686c%28Office.15%29.aspx) <br/> |O atributo **Id** retorna uma string que contém o identificador da pessoa.  <br/> |O atributo **Id** é o mesmo que o EwsId para a pessoa.  <br/> |
|[ContactId](http://msdn.microsoft.com/library/86f66275-1e39-48ed-bd89-ac3bffc465a7%28Office.15%29.aspx) <br/> |O atributo **Id** retorna uma string que contém o identificador do contato.  <br/> |O atributo **Id** é o mesmo que o EwsId para o contato.  <br/> |
|[GroupId](http://msdn.microsoft.com/library/656d9b9a-8a65-4a75-8466-5b0d96512dab%28Office.15%29.aspx) <br/> |O atributo **Id** retorna uma string que contém o identificador do grupo.  <br/> |O atributo **Id** é o mesmo que o EwsId para o grupo.  <br/> |
|[AssociatedCalendarItemId](http://msdn.microsoft.com/library/5b29898c-ea59-4e6a-914c-c011ec754032%28Office.15%29.aspx) <br/> |O atributo **Id** identifica o item de calendário que está associado um [MeetingMessage](http://msdn.microsoft.com/library/c95956a8-7505-44b4-bea4-11d1f5182796%28Office.15%29.aspx), [MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx), [MeetingResponse](http://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx)ou [MeetingCancellation](http://msdn.microsoft.com/library/a9c61f7f-2ecd-4b21-9dce-24d9f61aeeea%28Office.15%29.aspx).  <br/> |O atributo **Id** é o mesmo que o EwsId para o item de calendário.  <br/> |
|[UserConfigurationProperties](http://msdn.microsoft.com/library/c143a6ec-62ad-4d48-b844-b1ad88054bc1%28Office.15%29.aspx) <br/> |O valor de **identificação** para esse elemento Especifica a propriedade identifier.  <br/> |Esse identificador não mapear diretamente para o EwsId desde que ele um identificador de propriedade e não um item.  <br/> |
|[OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) <br/> |O atributo **RecurringMasterId** identifica o mestre de um item recorrente.  <br/> |O valor de **OccurrenceItemId** não é mapeado diretamente para o EwsId, mas o **RecurringMasterId** faz porque ele faz referência ao objeto de nível superior do item recorrente.  <br/> |
|[StoreEntryId](http://msdn.microsoft.com/library/f536e264-8c4d-4cc5-bab8-22a4fa38de39%28Office.15%29.aspx) <br/> |Contém o identificador do repositório do Exchange de um item.  <br/> |O valor de **StoreEntryId** não é mapeado para o EwsId, mas oferece a você o identificador do repositório onde os itens são mantidos.  <br/> |
   
## <a name="working-with-identifiers"></a>Trabalhando com identificadores
<a name="bk_WorkingWithIdentifiers"> </a>

O servidor do Exchange manipula identificadores em muitas maneiras diferentes. Considere o seguinte ao desenvolver seu aplicativo de EWS ou a API gerenciada de EWS:
  
- O valor do elemento **ItemID** para pastas e itens diferencia maiusculas de minúsculas. Se você observar a ID do item para uma pasta ou um item que é retornado pela [operação FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) (ou o método de API gerenciada de EWS [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ), você imagina que é uma duplicata do ID de outro item; No entanto, um ou mais caracteres no item IDs para os dois itens terão um caso de diferente. 
    
- Se você pretende armazenar a ID do item em um banco de dados para recuperar mais tarde, é recomendável que o tamanho do campo ser 512 bytes, para que ele seja grande o suficiente para armazenar o GUID.
    
- Não presuma que sua ID sempre será válida se você precisar recuperar o item mais tarde. Se um item é movido no repositório, a ID pode alterar devido à forma que um movimento é manipulado. Um item é realmente copiado, e uma nova ID é gerada e, em seguida, [o item original é excluído](deleting-items-by-using-ews-in-exchange.md).
    
- Identificadores no Exchange são opacos. Por exemplo, o EwsId é criado a partir de várias partes de informações que não são importantes para você, como o desenvolvedor, mas são importantes para o Exchange.
    
- Quando você trabalhar com itens no Exchange, outro valor deve ter em mente é o atributo **ChangeKey** . Esse valor, além de ID de item, é usado para rastrear o estado de um item. Sempre que um item for alterado, uma nova chave de alteração é gerada. Quando você executa uma [operação UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx), por exemplo, você pode usar o atributo **ChangeKey** para informar o servidor que sua atualização está sendo aplicada para a versão mais atual do item. Se o outro aplicativo fez uma alteração no item que você está atualizando, as chaves de alteração não correspondem e não será capaz de realizar a atualização. 
    
## <a name="distinguished-folder-ids"></a>ID de pasta distinta
<a name="bk_DistinguishedFolderIds"> </a>

O Exchange inclui um número de pastas de caixa de correio predefinidos, cada um deles é atribuído a um identificador, conhecido como o ID de pasta distinta. Isso está definido pela enumeração [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) EWS Managed API e o elemento do EWS [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) . Você pode usar estas IDs de pasta distinta a mais fácil fazer referência a uma das pastas predefinidas. Por exemplo, para a pasta de caixa de entrada, você pode simplesmente usar "caixa de entrada" para o identificador, em vez de determinar o identificador de pasta. 
  
Outras pastas que você cria para organizar os itens de email também têm uma identificação exclusiva para essa pasta. Esse ID não altera mesmo se você alterar outras propriedades na pasta.
  
Você pode usar as IDs de pasta distinta como ponto de partida para acesso de representante. Quando você inicia o acesso de representante, você pode procurar itens ou pastas e fornecer a ID de pasta distinta para especificar onde pesquisar. Quando um usuário delegado acessa o servidor, um elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) que é um filho do elemento **DistinguishedFolderId** é usado para especificar explicitamente o delegado acessar a caixa de correio. 
  
## <a name="handling-errors"></a>Lidar com erros
<a name="bk_DealingWithErrors"> </a>

Cada programa é vinculado ao receber um erro de vez em seguida e aplicativos baseados no EWS não são exceção (trocadilhos). Você pode receber alguns erros relacionados ao identificador no elemento [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) EWS ou como parte do da enumeração [ServiceError](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) API gerenciada de EWS. 
  
Os seguintes erros podem ocorrer na sua API gerenciada de EWS ou aplicativos do EWS. Se você estiver trabalhando com um aplicativo do EWS Managed API, os erros são geralmente problemas com valores de propriedade; para aplicativos do EWS, os erros estão associados a valores de elemento XML ou operações.
  
**Tabela 2. Erros relacionados a identificador**

|**Erro**|**Ocorre quando …**|**Descrição**|
|:-----|:-----|:-----|
|ErrorCalendarCannotUseIdForOccurrenceId  <br/> |O valor do **OccurenceID** não corresponde a um item de calendário recorrente válido.  <br/> |O valor da **OccurenceId** que foi especificado na solicitação pode ser válido na estrutura, mas a solicitação não pôde associá-lo a um mestre recorrente existente. O item recorrente pode ser removido do calendário. Verifique se o item ainda existe e que você está usando o identificador correto.  <br/> |
|ErrorCalendarCannotUseIdForRecurringMasterId  <br/> |O atributo **RecurringMasterId** não corresponde a uma ocorrência válida do elemento **OccurrenceId** .  <br/> |O valor da **RecurringMasterId** que foi especificado na solicitação pode ser válido na estrutura, mas a solicitação não pôde associá-lo a uma ocorrência existente do item. A ocorrência do item pode ser removida do calendário. Verifique se o item ainda existe e que você está usando o identificador correto.  <br/> |
|ErrorCannotUseFolderIdForItemId  <br/> |A **ID** passado representa uma pasta em vez de um item.  <br/> |O identificador pode ser válido no formato, mas não o que o servidor estava esperando para a operação. Verifique se você está fazendo referência o identificador correto para a operação.  <br/> |
|ErrorCannotUseItemIdForFolderId  <br/> |A **ID** passado na representa um item em vez de uma pasta.  <br/> |O identificador pode ser válido no formato, mas não o que o servidor estava esperando para a operação. Verifique se você está fazendo referência a correta **identificação** para a operação.  <br/> |
|ErrorChangeKeyRequiredForWriteOperations  <br/> |Uma chave válida de alteração deve ser fornecida quando você executa determinadas operações de atualização.  <br/> |Ou você omitido um valor **ChangeKey** quando você solicitou uma atualização, ou a chave de alteração estava incorreta. Verifique se você tem a chave de alteração correto quando você realizar operações de atualização.  <br/> |
|ErrorInvalidAttachmentId  <br/> |O anexo não foi encontrado dentro da coleção de anexos para o item.  <br/> |Você pode receber este código de resposta, se você tiver uma **identificação** do anexo e, em seguida, o anexo é excluído e você tentar chamar a [operação GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) na identificação de anexo. Verificar a existência de anexo na coleção de anexos.  <br/> |
|ErrorInvalidChangeKey  <br/> |Uma chave de alteração inválido foi passada.  <br/> |Observe que muitas operações e métodos não exigem uma chave de alteração a serem passados. No entanto, se você fornecer uma chave de alteração, ela deve ser válida, embora ele não necessariamente precisa ser atualizado.  <br/> |
|ErrorInvalidFolderId  <br/> |O **ID** da pasta está corrompido.  <br/> |Verifique se que você tem um identificador válido e formatado corretamente.  <br/> |
|ErrorInvalidId  <br/> |A estrutura da chave **ID** e/ou alteração é inconsistente internamente.  <br/> |Exchange encontrou um problema com a **ID** depois que ela foi analisada. Talvez tenha ocorrido um erro na conversão. Isso pode ocorrer, por exemplo, se você tiver um **IdFormatType.HexEntryId** para um item no Outlook, mas você pode convertê-lo em um pensamento EwsId era um formato **IdFormatType.EntryId** . Verifique se que você usar o tipo de conversão correta.  <br/> |
|ErrorInvalidIdEmpty  <br/> |O aplicativo especificado uma **identificação** que está vazio.  <br/> |Seu aplicativo passadas em uma sequência vazia para o identificador. Verifique se que você tem um identificador válido e formatado corretamente.  <br/> |
|ErrorInvalidIdMalformed  <br/> |A estrutura de **ID** é inconsistente internamente.  <br/> |Exchange encontrou um problema com a **ID** depois que ela foi analisada. A ID pode não ter sido convertida corretamente. Verifique se que você usar o tipo de conversão correta.  <br/> |
|ErrorInvalidIdMalformedEwsLegacyIdFormat  <br/> |Uma pasta ou item **ID** que está usando o formato do Exchange 2007 foi especificado para uma solicitação com uma versão do Exchange 2007 SP1 ou posterior.  <br/> |Você não pode usar as IDs de 2007 do Exchange no Exchange 2007 SP1 ou posteriores solicitações. Você deve usar a operação de EWS [ConvertId](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx) ou o método de API gerenciada de EWS [ConvertId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.convertid%28v=exchg.80%29.aspx) para convertê-los primeiro.  <br/> |
|ErrorInvalidIdNotAnItemAttachmentId  <br/> |A propriedade **AttachmentId** não faz referência a um anexo do item.  <br/> |O identificador pode ser válido no formato, mas não o que o servidor estava esperando para a operação. Verifique se você está fazendo referência o identificador correto para a operação.  <br/> |
|ErrorInvalidIdReturnedByResolveNames  <br/> |Um contato na sua caixa de correio está corrompido.  <br/> |A operação de EWS [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) ou o método [ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) EWS Managed API retornou um ou mais identificadores, mas não são válidos. Talvez você precise recriar o contato.  <br/> |
|ErrorInvalidIdStoreObjectIdTooLong  <br/> |A estrutura de **ID** é inconsistente internamente.  <br/> |Exchange encontrou um problema com a **ID** depois que ela foi analisada. A **ID** pode não ter sido convertidos corretamente. Verifique se que você usar o tipo de conversão correta.  <br/> |
|ErrorInvalidIdTooManyAttachmentLevels  <br/> |As hierarquias de anexo excederem o número máximo de 255 níveis de profundidade.  <br/> |O valor da propriedade **AttachmentId** que foi especificado na solicitação pode ser válido na estrutura, mas o anexo solicitado é muito profundo na hierarquia. Seu código pode ter tentado anexar um item além do limite de 255 níveis.  <br/> |
|ErrorInvalidImContactId  <br/> |Esse erro pode ser retornado quando o contato não pode ser encontrado no grupo de mensagens Instantâneas quando você usar a [operação RemoveImContactFromGroup](http://msdn.microsoft.com/library/a190bbec-c71b-4e6a-880b-55854c724d8c%28Office.15%29.aspx). Esse erro se aplica aos clientes que visam o Exchange Online e versões do Exchange, começando com o Exchange 2013.  <br/> |O valor da propriedade **ContactId** que foi especificado na solicitação pode ser válido na estrutura, mas nenhum contato na caixa de correio corresponde a esta estrutura. O contato pode ter sido removido já.  <br/> |
|ErrorInvalidImGroupId  <br/> |Esse erro pode ser retornado quando o grupo não pode ser encontrado na caixa de correio quando você usar a [operação RemoveImGroup](http://msdn.microsoft.com/library/5e788016-68e0-4a3f-9243-03f6b6c6b389%28Office.15%29.aspx). Esse erro se aplica aos clientes que visam o Exchange Online e versões do Exchange, começando com o Exchange 2013.  <br/> |O valor da propriedade **GroupId** que foi especificado na solicitação pode ser válido na estrutura, mas nenhum grupo na caixa de correio coincida com essa estrutura. O grupo pode ter sido removido já.  <br/> |
|ErrorInvalidReferenceItem  <br/> |O identificador do item referenciado não é um **MessageType** **ExchangeWebServices.CalendarItemTypeType**ou um de seus descendentes. O identificador do item de referência é para um objeto **CalendarItemType** e o organizador está tentando responder ou responder a todos.  <br/> |O identificador pode ser válido no formato, mas não o que o servidor estava esperando para a operação. Verifique se você está fazendo referência o identificador correto para a operação.  <br/> |
|ErrorMissingManagedFolderId  <br/> |A propriedade IDs de política, a marca de propriedade 0x6732, para a pasta está falta.  <br/> |A pasta está corrompida. Considere recriá-la.  <br/> |
   
## <a name="converting-identifiers"></a>Convertendo identificadores
<a name="bk_ConvertingIdentifiers"> </a>

Você pode precisar converter um identificador de um formato para outro. Por exemplo, talvez seja necessário converter um identificador do EWS externo, como um identificador que vêm de uma conexão de MAPI, em um formato que o aplicativo pode usar. Para fazer isso, você pode usar a operação de EWS [ConvertId](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx) ou o método de API gerenciada de EWS [ConvertId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.convertid%28v=exchg.80%29.aspx) . 
  
Por exemplo, uma EntryID é um identificador exclusivo gerado pelo armazenamento de mensagens MAPI atribuída pela loja quando o item é salvo. Para usar uma EntryID em seu aplicativo, você precisará primeiro convertê-lo em um EwsId. 
  
Outlook Web App usa seu próprio versão dos identificadores, chamado OwaId, em URLs para acessar pastas e itens. Se seu aplicativo precisar acessar itens no Outlook Web App, você precisará converter o OwaId em um EwsId.
  
Você pode usar o método ou a operação **ConvertId** para converter vários formatos de identificador diferente. 
  
**Tabela 3. Formatos de identificador conversível no Exchange**

|**Format**|**Descrição**|
|:-----|:-----|
|EwsLegacyId  <br/> |O EwsId que se aplica ao Exchange 2007.  <br/> |
|EwsId  <br/> |O EwsId que se aplica ao Exchange Online e versões do Exchange, começando com o Exchange 2007 SP1.  <br/> |
|StoreId  <br/> |O identificador do repositório do Exchange onde as pastas e itens são armazenados.  <br/> |
|OwaId  <br/> |O identificador do Outlook Web App usado com o Outlook Web App no Exchange 2007 e Exchange 2010. <br/><br/>**Observação**: o Exchange Online e versões do Exchange, começando com o Exchange 2013 usam o EwsId para o Outlook Web App.           |
|EntryId  <br/> |Um identificador MAPI que normalmente é conhecido como a propriedade **PR_ENTRYID** de uma mensagem MAPI.  <br/> |
|HexEntryId  <br/> |Uma representação hexadecimal codificado da propriedade **PR_ENTRYID** que é usada para o identificador de evento de calendário de disponibilidade. Isso também é o formato do identificador que o Outlook usa.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)  
- [Operação ConvertId](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx)  
- [Enumeração ServiceError](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) 
- [Excluindo itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md)
    

