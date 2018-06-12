---
title: Operações do EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exchange
api_type:
- schema
ms.assetid: cf6fd871-9a65-4f34-8557-c8c71dd7ce09
description: Encontre informações sobre as operações de EWS que estão disponíveis no Exchange.
ms.openlocfilehash: c56c3be746138cec251836fcb61ee3738d168869
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752134"
---
# <a name="ews-operations-in-exchange"></a>Operações do EWS no Exchange

Encontre informações sobre as operações de EWS que estão disponíveis no Exchange.
  
Serviços Web do Exchange (EWS) oferece muitas operações que permitem acessar informações do armazenamento do Exchange. Os artigos nesta seção fornecem informações sobre a estrutura geral de solicitações, respostas e mensagens de resposta de erro para operações de EWS, bem como exemplos XML para cada operação. Eles fornecem uma visão geral das estruturas de mensagem que são enviados entre o cliente e o servidor. Você pode usar essas informações para depurar estruturas de mensagem e encontrar informações sobre o que você pode fazer em uma solicitação EWS. Para obter mais informações sobre o que o representa de estrutura XML, consulte - [os elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md).
  
Todas as funcionalidades do EWS é associada uma versão do esquema. Novas versões de esquema do EWS são introduzidas em novas versões do Exchange Server ou o Exchange Online. O elemento [RequestServerVersion](requestserverversion.md) contém um atributo de **versão** que mapeia a versão do servidor para a versão do esquema. Este artigo fornece informações sobre quando cada operação foi introduzida. Funcionalidade específica dentro de uma operação pode exigir uma versão posterior do serviço. Os esquemas versionados são implementados para que os clientes que se adequam contra uma versão mais antiga do EWS funcionará com uma versão mais recente do EWS. 
  
Essas operações podem direcionar o ponto de extremidade do EWS que os serviços de sua caixa de correio. Você pode navegar até o ponto de extremidade do EWS usando uma URL semelhante na estrutura para http://<clientaccessserver>.com/ews/exchange.asmx, onde <clientaccessserver> é o servidor de acesso para cliente do Exchange que os serviços de sua caixa de correio. Você pode usar a descoberta automática para obter a URL para o servidor de acesso para cliente que os serviços de sua caixa de correio. Para obter mais informações sobre a descoberta automática, consulte [descoberta automática do Exchange](../exchange-web-services/autodiscover-for-exchange.md).
  
## <a name="ediscovery-operations"></a>operações de descoberta eletrônica
<a name="bk_eDiscovery"> </a>

As operações de descoberta eletrônica fornecem as operações de pesquisa para os armazenamentos legais e identificam os dados de caixa de correio que não podem ser indexados e retornados nos resultados da pesquisa de descoberta.
  
A tabela a seguir lista as operações de descoberta eletrônica.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação GetHoldOnMailboxes](getholdonmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação GetSearchableMailboxes](getsearchablemailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação SearchMailboxes](searchmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação SetHoldOnMailboxes](setholdonmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="exchange-mailbox-data-operations"></a>Operações de dados de caixa de correio do Exchange
<a name="bk_Exchange_mailbox_data"> </a>

As operações de dados de caixa de correio do Exchange permitem que os clientes manipular e organizar itens, pastas e anexos, bem como expansão de lista de distribuição e resolução de nome ambígua. Operações de dados de caixa de correio do Exchange incluem o item, pasta, anexo e operações de utilitários.
  
A tabela a seguir lista as operações de dados de caixa de correio do Exchange.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação ArchiveItem](archiveitem-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação CreateItem](createitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação CopyItem](copyitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação DeleteItem](deleteitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação FindItem](finditem-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação GetItem](getitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação MarkAllItemsAsRead](markallitemsasread-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação MoveItem](moveitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação SendItem](senditem-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação UpdateItem](updateitem-operation.md) <br/> |Exchange 2007  <br/> |
   
A tabela a seguir lista as operações de pasta de dados de caixa de correio Exchange.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação CreateFolder](createfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação CreateFolderPath](createfolderpath-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação CreateManagedFolder](createmanagedfolder-operation.md) <br/> |Exchange 2007. Essa funcionalidade tiver sido deemphasized nas versões do Exchange, começando com o Exchange 2010. Para obter mais informações sobre como migrar a usar marcas de retenção e políticas para gerenciamento de registros de mensagens, consulte [Migrate de pastas gerenciadas](http://technet.microsoft.com/en-us/library/dd298032%28v=exchg.141%29.aspx).  <br/> |
|[Operação CopyFolder](copyfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação DeleteFolder](deletefolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação EmptyFolder](emptyfolder-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação FindFolder](findfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação GetFolder](getfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação MoveFolder](movefolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação UpdateFolder](updatefolder-operation.md) <br/> |Exchange 2007  <br/> |
   
A tabela a seguir lista as operações de anexo de dados de caixa de correio Exchange.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação CreateAttachment](createattachment-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação GetAttachment](getattachment-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação DeleteAttachment](deleteattachment-operation.md) <br/> |Exchange 2007  <br/> |
   
A tabela a seguir lista as operações de lembrete de caixa de correio do Exchange.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação GetReminders](getreminders-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação PerformReminderAction](performreminderaction-operation.md) <br/> |Exchange 2013  <br/> |
   
A tabela a seguir lista as operações de conversa de dados de caixa de correio Exchange.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação ApplyConversationAction](applyconversationaction-operation.md) <br/> |Exchange 2010 Service Pack 1 (SP1)  <br/> |
|[Operação FindConversation](findconversation-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[Operação GetConversationItems](getconversationitems-operation.md) <br/> |Exchange 2013  <br/> |
   
A tabela a seguir lista as operações de utilitários de dados de caixa de correio Exchange.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação ConvertId](convertid-operation.md) <br/> |Exchange 2007 Service Pack 1  <br/> |
|[Operação ExpandDL](expanddl-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação GetUserPhoto](getuserphoto-operation.md) <br/> |Exchange 2013. Essa operação tem um REST e uma implementação SOAP.  <br/> |
|[Operação MarkAsJunk](markasjunk-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação ResolveNames](resolvenames-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação GetPasswordExpirationDate](getpasswordexpirationdate-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="availability-operations"></a>Operações de disponibilidade
<a name="bk_Availability"> </a>

As operações de disponibilidade melhorar o calendário e livre/ocupado compartilhamento experiência fornecendo mais seguras, atualizadas e ricas livre/ocupado informações. Informações de disponibilidade de dados são um componente essencial de agendamento de reuniões. As operações de disponibilidade fornecem uma base confiável para o planejamento efetivo. 
  
A tabela a seguir lista as operações de disponibilidade.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação GetUserAvailability](getuseravailability-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação GetRoomLists](getroomlists-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação GetRooms](getrooms-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação GetUserOofSettings](getuseroofsettings-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação SetUserOofSettings](setuseroofsettings-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="bulk-transfer-operations"></a>Operações de transferência em massa
<a name="bk_bulk_transfer"> </a>

As operações de transferência em massa permitem que os clientes itens stream e sair de uma caixa de correio. 
  
A tabela a seguir lista as operações de transferência em massa.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação UploadItems](uploaditems-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[Operação ExportItems](exportitems-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="delegate-management-operations"></a>Operações de gerenciamento de representante
<a name="bk_delegate_management"> </a>

As operações de gerenciamento do representante permitem que os clientes adicionar, obter, atualizar e remover representantes de suas caixas de correio. 
  
A tabela a seguir lista as operações de gerenciamento do representante.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação AddDelegate](adddelegate-operation.md) <br/> |Exchange 2007 Service Pack 1 (SP1)  <br/> |
|[Operação GetDelegate](getdelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
|[Operação UpdateDelegate](updatedelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
|[Operação RemoveDelegate](removedelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
   
## <a name="inbox-rules-operations"></a>Operações de regras de caixa de entrada
<a name="bk_inbox_rules"> </a>

As operações de regras de caixa de entrada permitem que os clientes obter as regras de caixa de entrada e atualizá-los para mensagens no servidor. As regras de caixa de entrada são conjuntos de condições e ações associadas que permitem que os clientes automaticamente organizar, categorizar e agem nas mensagens, como as mensagens são entregues a uma pasta. 
  
A tabela a seguir lista as operações de regras de caixa de entrada.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação GetInboxRules](getinboxrules-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[Operação UpdateInboxRules](updateinboxrules-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="mail-app-management-operations"></a>Operações de gerenciamento de aplicativo de email
<a name="bk_mail_apps"> </a>

As operações de gerenciamento de aplicativo de email permitem gerenciar aplicativos de email do Outlook. Você pode usar essas operações para instalar, desinstalar, desabilite e obter informações sobre aplicativos de email que estão disponíveis para o Outlook Web App e Outlook 2013.
  
A tabela a seguir lista as operações de gerenciamento de aplicativo de email.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação DisableApp](disableapp-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação GetAppManifests](getappmanifests-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação GetAppMarketplaceUrl](getappmarketplaceurl-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação GetClientAccessToken](getclientaccesstoken-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação InstallApp](installapp-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação UninstallApp](uninstallapp-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="mail-tips-operation"></a>Operação de dicas de email
<a name="bk_mail_tips"> </a>

A operação de dicas de email permite que os clientes para solicitar informações do servidor sobre caixas de correio de destinatários quando um autor está redigindo uma mensagem. A tabela a seguir lista a operação de dicas de email.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação GetMailTips](getmailtips-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="message-tracking-operations"></a>Operações de rastreamento de mensagem
<a name="bk_message_tracking"> </a>

As operações de rastreamento de mensagem permitem que os clientes para localizar mensagens que atendam aos critérios especificados e para obter informações de controle detalhado sobre cada mensagem em uma relatório de controle de mensagens. 
  
A tabela a seguir lista as operações de controle de mensagens.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação FindMessageTrackingReport](findmessagetrackingreport-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="notification-operations"></a>Operações de notificação
<a name="bk_notification"> </a>

As operações de notificação notificar o aplicativo cliente de eventos que estão associadas a itens e pastas em uma caixa de correio especificada. O modelo de assinatura pode ser baseado em push, baseado em extração ou baseada em streaming. 
  
A tabela a seguir lista as operações de notificação.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação GetEvents](getevents-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação GetStreamingEvents](getstreamingevents-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[Inscrever-se a operação](subscribe-operation.md) <br/> |Exchange 2007  <br/> |
|[Cancelar a operação](unsubscribe-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="persona-operations"></a>Operações de pessoa
<a name="bk_personas"> </a>

As operações de pessoa oferecem uma interface para encontrar e obter informações sobre um contato vinculado. A tabela a seguir lista as operações de pessoa.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação FindPeople](findpeople-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação GetPersona](getpersona-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="retention-policy-operation"></a>Operação de política de retenção
<a name="bk_retention_policy"> </a>

A operação de política de retenção fornece uma lista de todas as marcas de retenção vinculadas a política de retenção do usuário. 
  
A tabela a seguir lista a operação de política de retenção.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação GetUserRetentionPolicyTags](getuserretentionpolicytags-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="service-configuration-operation"></a>Operação de configuração de serviço
<a name="bk_service_config"> </a>

A operação de configuração de serviço permite que os clientes obter informações de configuração para os serviços de Unificação de mensagens, as regras de proteção, dicas de política e dicas de email. 
  
A tabela a seguir lista a operação de configuração de serviço.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação GetServiceConfiguration](getserviceconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="sharing-operations"></a>Operações de compartilhamento
<a name="bk_sharing"> </a>

As operações de compartilhamento permitem que os clientes compartilhem dados de calendário e dados de contatos. 
  
A tabela a seguir lista as operações de compartilhamento.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[CreateItem (AcceptSharingInvitation)](createitem-acceptsharinginvitation.md) <br/> |Exchange 2010. Embora a operação **CreateItem** é aplicável a todas as versões do EWS, o objeto de resposta de **AcceptSharingInvitation** só é aplicável a EWS nas versões do Exchange, começando com o Exchange 2010.  <br/> |
|[Operação GetSharingFolder](getsharingfolder-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação GetSharingMetadata](getsharingmetadata-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação RefreshSharingFolder](refreshsharingfolder-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="synchronization-operations"></a>Operações de sincronização
<a name="bk_synchronization"> </a>

As operações de sincronização fornecem uma cópia de cache sincronizada unidirecional de pastas e itens de um usuário. 
  
A tabela a seguir lista as operações de sincronização.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação SyncFolderHierarchy](syncfolderhierarchy-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação SyncFolderItems](syncfolderitems-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="time-zone-operation"></a>Operação de fuso horário
<a name="bk_timezone"> </a>

A operação de fuso horário permite que os clientes obter uma lista das definições de fuso horário que são suportados pelo servidor. 
  
A tabela a seguir lista a operação de fuso horário.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação GetServerTimeZones](getservertimezones-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="unified-messaging-operations"></a>Operações do Unified Messaging
<a name="bk_um"> </a>

As operações de Unificação de mensagens permitem que os clientes para ler informações sobre propriedades de Unificação de mensagens e reproduzir mensagens de voz por telefone. 
  
A tabela a seguir lista as operações de Unificação de mensagens.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação DisconnectPhoneCall](disconnectphonecall-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação GetPhoneCallInformation](getphonecallinformation-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação de PlayOnPhone (EWS)](playonphone-operation-ews.md) <br/> |Exchange 2010  <br/> |
   
Use a [operação GetServiceConfiguration](getserviceconfiguration-operation.md) para obter as informações de configuração de Unificação de mensagens para uma caixa de correio. Use o serviço de web de Unificação de mensagens para aplicativos de Unificação de mensagens que visam o Exchange 2007. Para obter mais informações, consulte [referência de serviço da web de Unificação de mensagens do Exchange](unified-messaging-web-service-reference-for-exchange.md).
  
## <a name="unified-contact-store-operations"></a>Operações de armazenamento de contato unificadas
<a name="bk_ucs"> </a>

O repositório unificado de contatos fornece uma experiência consistente de contato em produtos do Office e atua como um ponto de integração para aplicativos de terceiros para usar o mesmo armazenamento de contato. Permite que usuários e aplicativos armazenar, gerenciar e acessar informações de contato e disponibilizá-lo globalmente entre o Lync, Exchange 2013, Outlook, Outlook Web App e qualquer outro aplicativo que implementa o acesso ao repositório unificado de contatos. O Exchange é o repositório de conteúdo para a experiência do repositório unificado de contatos.
  
A tabela a seguir lista as operações do repositório unificado de contatos.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação AddNewImContactToGroup](addnewimcontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação AddImContactToGroup](addimcontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação AddImGroup](addimgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação AddNewTelUriContactToGroup](addnewteluricontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação AddDistributionGroupToImList](adddistributiongrouptoimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação GetImItemList](getimitemlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação GetImItems](getimitems-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação RemoveContactFromImList](removecontactfromimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação RemoveImContactFromGroup](removeimcontactfromgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação RemoveDistributionGroupFromImList](removedistributiongroupfromimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação RemoveImGroup](removeimgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação SetImGroup](setimgroup-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="user-configuration-operations"></a>Operações de configuração do usuário
<a name="bk_user_config"> </a>

As operações de configuração do usuário permitem que os clientes criar, excluir, obter e atualizar informações de configuração do usuário. 
  
A tabela a seguir lista as operações de configuração do usuário.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação CreateUserConfiguration](createuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação DeleteUserConfiguration](deleteuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação GetUserConfiguration](getuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação UpdateUserConfiguration](updateuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="see-also"></a>Confira também

- [Explorar a API Gerenciada pelo EWS, EWS e serviços Web no Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Start using web services in Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Descoberta Automática do Exchange](../exchange-web-services/autodiscover-for-exchange.md)
    

