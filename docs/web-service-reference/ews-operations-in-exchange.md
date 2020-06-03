---
title: Operações do EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- Exchange
api_type:
- schema
ms.assetid: cf6fd871-9a65-4f34-8557-c8c71dd7ce09
description: Encontre informações sobre as operações do EWS disponíveis no Exchange.
localization_priority: Priority
ms.openlocfilehash: 143903d9198a7e31e876adcbbb336df34ecf01fa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526120"
---
# <a name="ews-operations-in-exchange"></a>Operações do EWS no Exchange

Encontre informações sobre as operações do EWS disponíveis no Exchange.
  
Os serviços Web do Exchange (EWS) oferecem muitas operações que permitem acessar informações do armazenamento do Exchange. Os artigos desta seção fornecem informações sobre a estrutura geral das solicitações, respostas e mensagens de resposta de erro para operações do EWS, bem como exemplos XML para cada operação. Eles fornecem uma visão geral das estruturas de mensagens que são enviadas entre o cliente e o servidor. Você pode usar essas informações para depurar estruturas de mensagens e localizar informações sobre o que você pode fazer em uma solicitação do EWS. Para obter mais informações sobre o que a estrutura XML representa, consulte: [elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md).
  
Toda a funcionalidade do EWS está associada a uma versão do esquema. Novas versões de esquema do EWS são introduzidas em novas versões do Exchange Server ou Exchange Online. O elemento [RequestServerVersion](requestserverversion.md) contém um atributo **version** que mapeia a versão do servidor para a versão do esquema. Este artigo fornece informações sobre quando cada operação foi introduzida. A funcionalidade específica dentro de uma operação pode exigir uma versão mais recente do serviço. Os esquemas com controle de versão são implementados para que os clientes criados em uma versão mais antiga do EWS funcionem com uma versão mais recente do EWS. 
  
Essas operações podem ser direcionadas para o ponto de extremidade do EWS que Services sua caixa de correio. Você pode navegar até o ponto de extremidade do EWS usando uma URL semelhante a http:// <clientaccessserver> . com/EWS/Exchange. asmx, onde <clientaccessserver> é o servidor de acesso para cliente do Exchange que Services sua caixa de correio. Você pode usar a descoberta automática para obter a URL para o servidor de acesso para cliente que é o serviço de sua caixa de correio. Para obter mais informações sobre a descoberta automática, confira [descoberta automática do Exchange](../exchange-web-services/autodiscover-for-exchange.md).
  
## <a name="ediscovery-operations"></a>operações de descoberta eletrônica
<a name="bk_eDiscovery"> </a>

As operações de descoberta eletrônica fornecem operações de pesquisa para isenções legais e identificam os dados de caixa de correio que não podem ser indexados e retornados nos resultados da pesquisa de descoberta.
  
A tabela a seguir lista as operações de descoberta eletrônica.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação GetHoldOnMailboxes](getholdonmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação GetSearchableMailboxes](getsearchablemailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação SearchMailboxes](searchmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação SetHoldOnMailboxes](setholdonmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="exchange-mailbox-data-operations"></a>Operações de dados de caixa de correio do Exchange
<a name="bk_Exchange_mailbox_data"> </a>

As operações de dados de caixa de correio do Exchange permitem que os clientes manipulem e organizem itens, pastas e anexos, bem como a resolução de nome ambígua e a expansão da lista de distribuição. As operações de dados de caixa de correio do Exchange incluem operações de item, pasta, anexo e utilitários.
  
A tabela a seguir lista as operações de dados de caixa de correio do Exchange.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação ArchiveItem](archiveitem-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação CreateItem](createitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação CopyItem](copyitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação DeleteItem](deleteitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação FindItem](finditem-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação GetItem](getitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação MarkAllItemsAsRead](markallitemsasread-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação MoveItem](moveitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação SendItem](senditem-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação UpdateItem](updateitem-operation.md) <br/> |Exchange 2007  <br/> |
   
A tabela a seguir lista as operações de pasta de dados de caixa de correio do Exchange.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação CreateFolder](createfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação createfolderpath](createfolderpath-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação CreateManagedFolder](createmanagedfolder-operation.md) <br/> |Exchange 2007. Essa funcionalidade foi enfatizada em versões do Exchange a partir do Exchange 2010. Para obter mais informações sobre como migrar para o uso de marcas e políticas de retenção para o gerenciamento de registros de mensagens, consulte [Migrate from Managed Folders](https://technet.microsoft.com/library/dd298032%28v=exchg.141%29.aspx).  <br/> |
|[Operação CopyFolder](copyfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação DeleteFolder](deletefolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação EmptyFolder](emptyfolder-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação FindFolder](findfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação GetFolder](getfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação MoveFolder](movefolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação UpdateFolder](updatefolder-operation.md) <br/> |Exchange 2007  <br/> |
   
A tabela a seguir lista as operações de anexo de dados da caixa de correio do Exchange.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação CreateAttachment](createattachment-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação GetAttachment](getattachment-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação DeleteAttachment](deleteattachment-operation.md) <br/> |Exchange 2007  <br/> |
   
A tabela a seguir lista as operações de lembrete da caixa de correio do Exchange.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação getlembretes](getreminders-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação PerformReminderAction](performreminderaction-operation.md) <br/> |Exchange 2013  <br/> |
   
A tabela a seguir lista as operações de conversa de dados de caixa de correio do Exchange.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação ApplyConversationAction](applyconversationaction-operation.md) <br/> |Exchange 2010 Service Pack 1 (SP1)  <br/> |
|[Operação FindConversation](findconversation-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[Operação GetConversationItems](getconversationitems-operation.md) <br/> |Exchange 2013  <br/> |
   
A tabela a seguir lista as operações dos utilitários de dados de caixa de correio do Exchange.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação convertid](convertid-operation.md) <br/> |Exchange 2007 Service Pack 1  <br/> |
|[Operação ExpandDL](expanddl-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação GetUserPhoto](getuserphoto-operation.md) <br/> |Exchange 2013. Essa operação tem uma implementação REST e SOAP.  <br/> |
|[Operação MarkAsJunk](markasjunk-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação ResolveNames](resolvenames-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação GetPasswordExpirationDate](getpasswordexpirationdate-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="availability-operations"></a>Operações de disponibilidade
<a name="bk_Availability"> </a>

As operações de disponibilidade aprimoram o calendário e a experiência de compartilhamento de disponibilidade fornecendo informações mais seguras, atualizadas e de disponibilidade avançadas. Os dados de disponibilidade são um componente crítico do agendamento de reuniões. As operações de disponibilidade fornecem uma base confiável para o agendamento efetivo. 
  
A tabela a seguir lista as operações de disponibilidade.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação GetUserAvailability](getuseravailability-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação GetRoomLists](getroomlists-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação getrooms](getrooms-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação GetUserOofSettings](getuseroofsettings-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação SetUserOofSettings](setuseroofsettings-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="bulk-transfer-operations"></a>Operações de transferência em massa
<a name="bk_bulk_transfer"> </a>

As operações de transferência em massa permitem que os clientes transmitam itens para dentro e para fora de uma caixa de correio. 
  
A tabela a seguir lista as operações de transferência em massa.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação UploadItems](uploaditems-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[Operação ExportItems](exportitems-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="delegate-management-operations"></a>Delegar operações de gerenciamento
<a name="bk_delegate_management"> </a>

As operações de gerenciamento de representante permitem que os clientes adicionem, obtenham, atualizem e removam representantes de suas caixas de correio. 
  
A tabela a seguir lista as operações de gerenciamento de representante.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação AddDelegate](adddelegate-operation.md) <br/> |Exchange 2007 Service Pack 1 (SP1)  <br/> |
|[Operação getdelegate](getdelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
|[Operação UpdateDelegate](updatedelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
|[Operação RemoveDelegate](removedelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
   
## <a name="inbox-rules-operations"></a>Operações de regras de caixa de entrada
<a name="bk_inbox_rules"> </a>

As operações de regras de caixa de entrada permitem aos clientes obter as regras de caixa de entrada e atualizá-las para mensagens no servidor. As regras de caixa de entrada são conjuntos de condições e ações associadas que permitem que os clientes organizem, categorizem e atuem automaticamente as mensagens, conforme as mensagens são entregues a uma pasta. 
  
A tabela a seguir lista as operações de regras de caixa de entrada.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação GetInboxRules](getinboxrules-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[Operação UpdateInboxRules](updateinboxrules-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="mail-app-management-operations"></a>Operações de gerenciamento de aplicativos de email
<a name="bk_mail_apps"> </a>

As operações de gerenciamento de aplicativos de email permitem gerenciar aplicativos de email para o Outlook. Você pode usar essas operações para instalar, desinstalar, desabilitar e obter informações sobre aplicativos de email disponíveis para o Outlook Web App e o Outlook 2013.
  
A tabela a seguir lista as operações de gerenciamento de aplicativos de email.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação DisableApp](disableapp-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação GetAppManifests](getappmanifests-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação GetAppMarketplaceUrl](getappmarketplaceurl-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação GetClientAccessToken](getclientaccesstoken-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação InstallApp](installapp-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação UninstallApp](uninstallapp-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="mail-tips-operation"></a>Operação de dicas de email
<a name="bk_mail_tips"> </a>

A operação de dicas de email permite que os clientes solicitem informações do servidor sobre caixas de correio de destinatário quando um autor estiver redigindo uma mensagem. A tabela a seguir lista a operação de dicas de email.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação](getmailtips-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="message-tracking-operations"></a>Operações de controle de mensagens
<a name="bk_message_tracking"> </a>

As operações de controle de mensagens permitem que os clientes encontrem mensagens que atendem a critérios específicos e obtenham informações de controle detalhadas sobre cada mensagem em um relatório de controle de mensagens. 
  
A tabela a seguir lista as operações de controle de mensagens.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação FindMessageTrackingReport](findmessagetrackingreport-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="notification-operations"></a>Operações de notificação
<a name="bk_notification"> </a>

As operações de notificação notificam o aplicativo cliente de eventos que estão associados a itens e pastas uma caixa de correio especificada. O modelo de assinatura pode ser baseado em força, recepção ou baseado em streaming. 
  
A tabela a seguir lista as operações de notificação.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação GetEvents](getevents-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação GetStreamingEvents](getstreamingevents-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[Operação Subscribe](subscribe-operation.md) <br/> |Exchange 2007  <br/> |
|[Cancelar a operação](unsubscribe-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="persona-operations"></a>Operações persona
<a name="bk_personas"> </a>

As operações persona fornecem uma interface para localizar e obter informações sobre um contato vinculado. A tabela a seguir lista as operações persona.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação FindPeople](findpeople-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação getpersona](getpersona-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="retention-policy-operation"></a>Operação de política de retenção
<a name="bk_retention_policy"> </a>

A operação de política de retenção fornece uma lista de todas as marcas de retenção vinculadas à política de retenção de um usuário. 
  
A tabela a seguir lista a operação de política de retenção.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação GetUserRetentionPolicyTags](getuserretentionpolicytags-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="service-configuration-operation"></a>Operação de configuração de serviço
<a name="bk_service_config"> </a>

A operação de configuração do serviço permite que os clientes obtenham informações de configuração para a Unificação de mensagens, regras de proteção, dicas de política e serviços de dicas de email. 
  
A tabela a seguir lista a operação de configuração do serviço.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação GetServiceConfiguration](getserviceconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="sharing-operations"></a>Operações de compartilhamento
<a name="bk_sharing"> </a>

As operações de compartilhamento permitem que os clientes compartilhem dados de calendário e de contatos. 
  
A tabela a seguir lista as operações de compartilhamento.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[CreateItem (AcceptSharingInvitation)](createitem-acceptsharinginvitation.md) <br/> |Exchange 2010. Embora a operação **CreateItem** seja aplicável a todas as versões do EWS, o objeto de resposta **AcceptSharingInvitation** só é aplicável ao EWS nas versões do Exchange a partir do Exchange 2010.  <br/> |
|[Operação GetSharingFolder](getsharingfolder-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação GetSharingMetadata](getsharingmetadata-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação RefreshSharingFolder](refreshsharingfolder-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="synchronization-operations"></a>Operações de sincronização
<a name="bk_synchronization"> </a>

As operações de sincronização fornecem uma cópia em cache sincronizada unidirecional de pastas e itens de um usuário. 
  
A tabela a seguir lista as operações de sincronização.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação SyncFolderHierarchy](syncfolderhierarchy-operation.md) <br/> |Exchange 2007  <br/> |
|[Operação SyncFolderItems](syncfolderitems-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="time-zone-operation"></a>Operação de fuso horário
<a name="bk_timezone"> </a>

A operação de fuso horário permite que os clientes obtenham uma lista de definições de fuso horário compatíveis com o servidor. 
  
A tabela a seguir lista a operação de fuso horário.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação GetServerTimeZones](getservertimezones-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="unified-messaging-operations"></a>Operações de Unificação de mensagens
<a name="bk_um"> </a>

As operações de Unificação de mensagens permitem que os clientes leiam informações sobre as propriedades da Unificação de mensagens e reproduzam mensagens de caixa postal por telefone. 
  
A tabela a seguir lista as operações de Unificação de mensagens.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação DisconnectPhoneCall](disconnectphonecall-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação GetPhoneCallInformation](getphonecallinformation-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação PlayOnPhone (EWS)](playonphone-operation-ews.md) <br/> |Exchange 2010  <br/> |
   
Use a [operação GetServiceConfiguration](getserviceconfiguration-operation.md) para obter as informações de configuração de Unificação de mensagens para uma caixa de correio. Use o serviço Web de Unificação de mensagens para aplicativos de Unificação de mensagens direcionados ao Exchange 2007. Para obter mais informações, consulte [Unified Messaging Web Service Reference for Exchange](unified-messaging-web-service-reference-for-exchange.md).
  
## <a name="unified-contact-store-operations"></a>Operações do repositório unificado de contatos
<a name="bk_ucs"> </a>

O repositório unificado de contatos fornece uma experiência de contato consistente entre os produtos do Office e atua como um ponto de integração para aplicativos de terceiros usarem o mesmo repositório de contatos. Ele permite que os usuários e aplicativos armazenem, gerenciem e acessem informações de contato e o disponibilizem globalmente entre o Lync, o Exchange 2013, o Outlook, o Outlook Web App e qualquer outro aplicativo que implemente o acesso ao repositório unificado de contatos. O Exchange é o repositório de conteúdo para a experiência do repositório unificado de contatos.
  
A tabela a seguir lista as operações do repositório unificado de contatos.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação AddNewImContactToGroup](addnewimcontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação AddImContactToGroup](addimcontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação AddImGroup](addimgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação AddNewTelUriContactToGroup](addnewteluricontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação AddDistributionGroupToImList](adddistributiongrouptoimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação GetImItemList](getimitemlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação GetImItems](getimitems-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação RemoveContactFromImList](removecontactfromimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação RemoveImContactFromGroup](removeimcontactfromgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação RemoveDistributionGroupFromImList](removedistributiongroupfromimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação RemoveImGroup](removeimgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Operação SetImGroup](setimgroup-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="user-configuration-operations"></a>Operações de configuração do usuário
<a name="bk_user_config"> </a>

As operações de configuração do usuário permitem que os clientes criem, excluam, obtenham e atualizem as informações de configuração do usuário. 
  
A tabela a seguir lista as operações de configuração do usuário.
  
|**Nome da operação**|**Introduzido no**|
|:-----|:-----|
|[Operação CreateUserConfiguration](createuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação DeleteUserConfiguration](deleteuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação GetUserConfiguration](getuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[Operação UpdateUserConfiguration](updateuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="see-also"></a>Confira também

- [Explorar os recursos da API gerenciada por EWS, EWS e serviços Web no Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Introdução ao uso dos serviços Web no Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Descoberta Automática do Exchange](../exchange-web-services/autodiscover-for-exchange.md)
    

