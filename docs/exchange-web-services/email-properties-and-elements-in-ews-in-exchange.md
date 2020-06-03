---
title: Propriedades e elementos de email no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 5266ff9f-d828-4ef4-b8ec-7b27d355c4c5
description: Saiba mais sobre a primeira classe e outras propriedades e elementos que você pode obter nas mensagens de email usando a API gerenciada do EWS ou o EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: d7f5c5e68dcd0c4fc481afa37b338a47b1fd2e96
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455433"
---
# <a name="email-properties-and-elements-in-ews-in-exchange"></a>Propriedades e elementos de email no EWS no Exchange

Saiba mais sobre a primeira classe e outras propriedades e elementos que você pode obter nas mensagens de email usando a API gerenciada do EWS ou o EWS no Exchange.
  
As mensagens de email têm mais de 50 Propriedades e obtendo as que você deseja, quando você quiser, podem ser confusas se você não souber onde procurar. O mais importante a saber mais sobre como trabalhar com propriedades e elementos de email é incluído no conjunto de propriedades e elementos de primeira classe que é retornado por cada um dos principais métodos e operações de recuperação. O conjunto de propriedades de primeira classe que é retornado varia com base no método de recuperação que você usa. Também é importante não ser enganado pelo valor de do elemento [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) EWS, que corresponde ao valor de enumeração [BasePropertySet. FirstClassMessageProperties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) na API gerenciada do EWS. Esse valor não inclui, de fato, todas as propriedades, apenas inclui as propriedades de primeira classe. 
  
## <a name="first-class-properties-and-elements-for-email-messages"></a>Propriedades e elementos de primeira classe para mensagens de email
<a name="bk_firstclass"> </a>

O conjunto de propriedades e elementos de primeira classe que são retornados pelo método de API gerenciada do EWS [EmailMessage. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) e a operação do EWS [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) é um pouco diferente do conjunto de propriedades e elementos de primeira classe que é retornado pelo método [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) da API gerenciada do EWS e pela operação do EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) . As propriedades de primeira classe retornadas pelo método **FindItems** e a operação **FindItem** são um subconjunto das propriedades retornadas pelo método **BIND** e a operação **GetItem** . A tabela 1 lista todas as propriedades de primeira classe retornadas pelo método **BIND** e a operação **GetItem** e especifica quais delas não são retornadas pelo método **FindItems** ou pela operação **FindItem** . Observe que você não pode estender o método **FindItems** ou a operação **FindItem** para recuperar propriedades e elementos adicionais, como **ToRecipients**, **CcRecipients**e **BccRecipients**. Se você precisar recuperar esses valores, use o método **FindItems** ou a operação **FindItem** para obter as IDs de item dos emails e, em seguida, use o método **BIND** ou a operação **GetItem** para recuperar as propriedades necessárias. Para obter exemplos de código que mostram como recuperar itens usando o método **BIND** ou **FindItems** , consulte [obter um item usando a API gerenciada do EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma). Para obter exemplos de código que mostram como recuperar itens usando as operações **GetItem** ou **FindItem** , consulte [obter um item usando o EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews).
  
As propriedades e elementos da primeira classe estão listados na tabela a seguir na ordem em que aparecem em uma resposta.
  
**Tabela 1. Elementos e propriedades de email de primeira classe**

|**Propriedade da API gerenciada do EWS**|**Elemento do EWS**|**Propriedade First-Class para o método **FindItems** ou a operação **FindItem** ?**|**Leitura-gravação ou somente leitura**|
|:-----|:-----|:-----|:-----|
|[Id](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) <br/> |[ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[ParentFolderId](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.parentfolderid%28v=exchg.80%29.aspx) <br/> |[ParentFolderId](https://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[ItemClass](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.itemclass%28v=exchg.80%29.aspx) <br/> |[ItemClass](https://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) <br/> |Sim  <br/> |Leitura-gravação  <br/> |
|[Assunto](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx) <br/> |[Assunto](https://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) <br/> |Sim  <br/> |Leitura-gravação  <br/> |
|[Sensitivity](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.sensitivity%28v=exchg.80%29.aspx) <br/> |[Sensitivity](https://msdn.microsoft.com/library/d872423a-c26e-4675-9028-23361fb4a43d%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[Body](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx) <br/> |[Body](https://msdn.microsoft.com/library/7851ea9b-9f87-4adc-a26f-7a27df4a9bca%28Office.15%29.aspx) <br/> |Não  <br/> |Leitura-gravação  <br/> |
|[Anexos](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) <br/> |[Anexos](https://msdn.microsoft.com/library/b470e614-34bb-44f0-8790-7ddbdcbbd29d%28Office.15%29.aspx) <br/> |Não  <br/> |Leitura-gravação  <br/> |
|[DateTimeReceived](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.datetimereceived%28v=exchg.80%29.aspx) <br/> |[DateTimeReceived](https://msdn.microsoft.com/library/8f489bd4-2434-4d0a-91fe-1b5ba7eb5765%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[Tamanho](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.size%28v=exchg.80%29.aspx) <br/> |[Tamanho](https://msdn.microsoft.com/library/966f4daf-c20e-49f8-aeb6-965f3e2da7c3%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[Categorias](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.categories%28v=exchg.80%29.aspx) <br/> |[Categorias](https://msdn.microsoft.com/library/d84d4927-b524-4e62-bf3d-1f12fec8c21a%28Office.15%29.aspx) <br/> |Não  <br/> |Leitura-gravação  <br/> |
|[Importance](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.importance%28v=exchg.80%29.aspx) <br/> |[Importance](https://msdn.microsoft.com/library/1557f59a-41f2-43fb-9ded-88f3ec5c76cb%28Office.15%29.aspx) <br/> |Sim  <br/> |Leitura-gravação  <br/> |
|[Inresponderto](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.inreplyto%28v=exchg.80%29.aspx) <br/> |[Inresponderto](https://msdn.microsoft.com/library/561b8941-1c26-4bbe-aa0f-b49ec8a79af5%28Office.15%29.aspx) <br/> |Sim  <br/> |Leitura-gravação  <br/> |
|[Isenviado](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.issubmitted%28v=exchg.80%29.aspx) <br/> |[Isenviado](https://msdn.microsoft.com/library/2399e27e-bd8c-46b6-a3aa-674842e098c9%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[IsDraft](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.isdraft%28v=exchg.80%29.aspx) <br/> |[IsDraft](https://msdn.microsoft.com/library/8b8d9cc9-a512-458a-94e4-af210ac83bd7%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[IsFromMe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.isfromme%28v=exchg.80%29.aspx) <br/> |[IsFromMe](https://msdn.microsoft.com/library/d3c5fbf0-a95c-46e5-890f-953e50ac49d6%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[IsResend](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.isresend%28v=exchg.80%29.aspx) <br/> |[IsResend](https://msdn.microsoft.com/library/8f758b6b-dcee-4f95-9d39-e4be2bd92961%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[IsUnmodified](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.isunmodified%28v=exchg.80%29.aspx) <br/> |[IsUnmodified](https://msdn.microsoft.com/library/8f758b6b-dcee-4f95-9d39-e4be2bd92961%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[Propriedadeinternetmessageheaders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.internetmessageheaders%28v=exchg.80%29.aspx) <br/> |[Propriedadeinternetmessageheaders](https://msdn.microsoft.com/library/4dcf8671-96df-4a2d-9836-7e8e3a67e0db%28Office.15%29.aspx) <br/> |Não  <br/> |Somente leitura  <br/> |
|[DateTimeSent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.datetimesent%28v=exchg.80%29.aspx) <br/> |[DateTimeSent](https://msdn.microsoft.com/library/81784ef3-8912-4d63-8502-73419a906999%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[DateTimeCreated](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.datetimecreated%28v=exchg.80%29.aspx) <br/> |[DateTimeCreated](https://msdn.microsoft.com/library/42ae0067-4688-49d9-93c5-c4dbeb54cee1%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[AllowedResponseActions](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.allowedresponseactions%28v=exchg.80%29.aspx) <br/> |[ResponseObjects](https://msdn.microsoft.com/library/ad29e064-3f3d-4b7b-aa4c-9ec27326381d%28Office.15%29.aspx) <br/> |Não  <br/> |Somente leitura  <br/> |
|[ReminderDueBy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.reminderdueby%28v=exchg.80%29.aspx) <br/> |[ReminderDueBy](https://msdn.microsoft.com/library/e28a0485-86af-4a4e-a2ba-3ad2d4ebff6f%28Office.15%29.aspx) <br/> |Sim  <br/> |Leitura-gravação  <br/> |
|[ReminderSet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.isreminderset%28v=exchg.80%29.aspx) <br/> |[ReminderIsSet](https://msdn.microsoft.com/library/fa366afe-77a0-4c14-9edb-ffc9699131ba%28Office.15%29.aspx) <br/> |Sim  <br/> |Leitura-gravação  <br/> |
|[ReminderMinutesBeforeStart](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.reminderminutesbeforestart%28v=exchg.80%29.aspx) <br/> |[ReminderMinutesBeforeStart](https://msdn.microsoft.com/library/65ea14bc-5f19-48cc-aef1-46227e06f5f5%28Office.15%29.aspx) <br/> |Sim  <br/> |Leitura-gravação  <br/> |
|[DisplayCc](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.displaycc%28v=exchg.80%29.aspx) <br/> |[DisplayCc](https://msdn.microsoft.com/library/af386e06-80f3-42c7-8b3c-1f7993c49d10%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[DisplayTo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.displayto%28v=exchg.80%29.aspx) <br/> |[DisplayTo](https://msdn.microsoft.com/library/16a0b22d-063b-417c-8aba-efcf9490b072%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[HasAttachments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) <br/> |[HasAttachments](https://msdn.microsoft.com/library/538b7a85-11d7-4daa-8458-09b540760e8b%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[Cultura](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.culture%28v=exchg.80%29.aspx) <br/> |[Cultura](https://msdn.microsoft.com/library/71bd62c6-3fec-48db-9a5e-02121e9bc20b%28Office.15%29.aspx) <br/> |Sim  <br/> |Leitura-gravação  <br/> |
|[EffectiveRights](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.effectiverights%28v=exchg.80%29.aspx) <br/> |[EffectiveRights](https://msdn.microsoft.com/library/bf5278eb-3a1a-4d27-9d16-b8be043bb023%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[LastModified](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.lastmodifiedname%28v=exchg.80%29.aspx) <br/> |[LastModified](https://msdn.microsoft.com/library/4f1a90c1-e27e-4e16-93c3-e79d4cb720d1%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[LastModifiedTime](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.lastmodifiedtime%28v=exchg.80%29.aspx) <br/> |[LastModifiedTime](https://msdn.microsoft.com/library/6db2cabc-e7f4-4d71-962b-789de6a192a4%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[Isassociated](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.isassociated%28v=exchg.80%29.aspx) <br/> |[Isassociated](https://msdn.microsoft.com/library/637f0798-6680-487f-bcbf-aaddc4a74186%28Office.15%29.aspx) <br/> |Sim  <br/> |Leitura-gravação  <br/> |
|[WebClientReadFormQueryString](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.webclientreadformquerystring%28v=exchg.80%29.aspx) <br/> |[WebClientReadFormQueryString](https://msdn.microsoft.com/library/13e8871a-32a6-4bb9-9493-864c4c07efff%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[WebClientEditFormQueryString](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.webclienteditformquerystring%28v=exchg.80%29.aspx) <br/> |[WebClientEditFormQueryString](https://msdn.microsoft.com/library/9e571021-d58f-424b-8db2-48cf683533dc%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[ConversationId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.conversationid%28v=exchg.80%29.aspx) <br/> |[ConversationId](https://msdn.microsoft.com/library/d5f1ddb3-9af3-4677-a6ba-111b304a951e%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[Flag](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.flag%28v=exchg.80%29.aspx) <br/> |[Flag](https://msdn.microsoft.com/library/7b47bc74-a60d-4308-8674-5d52444a1753%28Office.15%29.aspx) <br/> |Sim  <br/> |Leitura-gravação  <br/> |
|[InstanceKey](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.instancekey%28v=exchg.80%29.aspx) <br/> |[InstanceKey](https://msdn.microsoft.com/library/bb4dbe9b-aea0-4527-b7d6-e928066caf38%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[EntityExtractionResult](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.entityextractionresult%28v=exchg.80%29.aspx) <br/> |[EntityExtractionResult](https://msdn.microsoft.com/library/643b99ab-ff90-4411-864c-1077623028d6%28Office.15%29.aspx) <br/> |Não  <br/> |Somente leitura  <br/> |
|[Sender](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.sender%28v=exchg.80%29.aspx) <br/> |[Sender](https://msdn.microsoft.com/library/26d1a46e-e1d3-44b8-a02d-fa6f83aa5cda%28Office.15%29.aspx) <br/> |Sim  <br/> |Leitura-gravação  <br/> |
|[ToRecipients](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx) <br/> |[ToRecipients](https://msdn.microsoft.com/library/72dc3be8-30bb-4ae1-acf4-fb94ff490631%28Office.15%29.aspx) <br/> |Não  <br/> |Somente leitura  <br/> |
|[CcRecipients](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.ccrecipients%28v=exchg.80%29.aspx) <br/> |[CcRecipients](https://msdn.microsoft.com/library/5c20ec3a-0bee-4e67-b220-586ed0d601c9%28Office.15%29.aspx) <br/> |Não  <br/> |Somente leitura  <br/> |
|[BccRecipients](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bccrecipients%28v=exchg.80%29.aspx) <br/> |[BccRecipients](https://msdn.microsoft.com/library/c4e05168-d36b-4740-a526-4b7da53553c1%28Office.15%29.aspx) <br/> |Não  <br/> |Somente leitura  <br/> |
|[IsReadReceiptRequested](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.isreadreceiptrequested%28v=exchg.80%29.aspx) <br/> |[IsReadReceiptRequested](https://msdn.microsoft.com/library/7ab6edd5-c7ed-4701-8de3-d7dc7ecfa9c2%28Office.15%29.aspx) <br/> |Sim  <br/> |Leitura-gravação  <br/> |
|[IsDeliveryReceiptRequested](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.isdeliveryreceiptrequested%28v=exchg.80%29.aspx) <br/> |[IsDeliveryReceiptRequested](https://msdn.microsoft.com/library/97776b7e-942c-4663-8277-165d64364daa%28Office.15%29.aspx) <br/> |Sim  <br/> |Leitura-gravação  <br/> |
|[ConversationIndex](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.conversationindex%28v=exchg.80%29.aspx) <br/> |[ConversationIndex](https://msdn.microsoft.com/library/fdf47e22-8d93-4ae4-883b-0c9f07f48724%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[ConversationTopic](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.conversationtopic%28v=exchg.80%29.aspx) <br/> |[ConversationTopic](https://msdn.microsoft.com/library/46cacf42-4039-4c8a-9b20-c42cdd9f2760%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[De](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.from%28v=exchg.80%29.aspx) <br/> |[De](https://msdn.microsoft.com/library/5a52d644-3677-4049-874c-12bd5c3080dc%28Office.15%29.aspx) <br/> |Sim  <br/> |Leitura-gravação  <br/> |
|[InternetMessageId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.internetmessageid%28v=exchg.80%29.aspx) <br/> |[InternetMessageId](https://msdn.microsoft.com/library/a5a9563f-e761-4658-9957-0e13566f6a35%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[IsRead](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.isread%28v=exchg.80%29.aspx) <br/> |[IsRead](https://msdn.microsoft.com/library/161455d5-a870-4c99-b2eb-c759c538f1bc%28Office.15%29.aspx) <br/> |Sim  <br/> |Leitura-gravação  <br/> |
|[IsResponseRequested](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.isresponserequested%28v=exchg.80%29.aspx) <br/> |[IsResponseRequested](https://msdn.microsoft.com/library/8cb874ed-a538-4de6-ab22-2631092dcdd0%28Office.15%29.aspx) <br/> |Sim  <br/> |Leitura-gravação  <br/> |
|[ReplyTo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.replyto%28v=exchg.80%29.aspx) <br/> |[ReplyTo](https://msdn.microsoft.com/library/6b6ae792-e2c4-4aa0-95cb-b49b446f1e08%28Office.15%29.aspx) <br/> |Não  <br/> |Somente leitura  <br/> |
|[References](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.references%28v=exchg.80%29.aspx) <br/> |[References](https://msdn.microsoft.com/library/d78f9a48-cd24-452f-af65-4c01933227ce%28Office.15%29.aspx) <br/> |Sim  <br/> |Leitura-gravação  <br/> |
|[ReceivedBy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.receivedby%28v=exchg.80%29.aspx) <br/> |[ReceivedBy](https://msdn.microsoft.com/library/ac84c9c5-d2fe-4b6f-bf4d-0444131d835b%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
|[ReceivedRepresenting](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.receivedrepresenting%28v=exchg.80%29.aspx) <br/> |[ReceivedRepresenting](https://msdn.microsoft.com/library/1157b042-6dce-4cdc-9700-e22b749da39f%28Office.15%29.aspx) <br/> |Sim  <br/> |Somente leitura  <br/> |
   
## <a name="other-properties-and-elements-for-email-messages"></a>Outras propriedades e elementos para mensagens de email
<a name="bk_notfirstclass"> </a>

Nem todas as propriedades e elementos de email importantes são propriedades e elementos da primeira classe. Para obter as outras propriedades ou elementos, você precisa adicioná-los ao seu [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) se estiver usando a API gerenciada do EWS ou usar um caminho de propriedade para adicioná-los à chamada de operação do EWS. Por exemplo, para recuperar o corpo do texto e o conteúdo MIME de uma mensagem, crie seu **PropertySet** conforme mostrado para o método **BIND** ou **Load** . 
  
```cs
PropertySet(BasePropertySet.IdOnly, ItemSchema.TextBody, ItemSchema.MimeContent);
```

Ou se você estiver usando o EWS, adicione os elementos ao [elementoproperties](https://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) na sua solicitação de operação do **GetItem** , como mostrado. 
  
```XML
<t:AdditionalProperties>
    <t:FieldURI FieldURI="item:TextBody" />
    <t:FieldURI FieldURI="item:MimeContent" />
</t:AdditionalProperties>
```

 As propriedades **EmailMessage** herdadas do objeto do EWS Managed API [ServiceObject](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceobject%28v=exchg.80%29.aspx) não podem ser incluídas em um conjunto de propriedades para o método **BIND** ; no entanto, todas as propriedades **ServiceObject** são legíveis no objeto **EmailMessage** e são recuperadas pelo método **BIND** . 
  
**Tabela 2. Outras propriedades e elementos de email**

|**Propriedade da API gerenciada do EWS**|**Elemento do EWS**|**Leitura-gravação ou somente leitura**|
|:-----|:-----|:-----|
|[ArchiveTag](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.archivetag%28v=exchg.80%29.aspx) <br/> |[ArchiveTag](https://msdn.microsoft.com/library/c4cb0718-37cd-41aa-86e7-b492c4bb86aa%28Office.15%29.aspx) <br/> |Leitura-gravação  <br/> |
|[ExtendedProperties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.extendedproperties%28v=exchg.80%29.aspx) <br/> |[ExtendedProperty](https://msdn.microsoft.com/library/f9701409-b620-4afe-b9ee-4c1e95507af7%28Office.15%29.aspx) <br/> |Somente leitura  <br/> |
|[IconIndex](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.iconindex%28v=exchg.80%29.aspx) <br/> |[IconIndex](https://msdn.microsoft.com/library/92020822-2a86-4dfc-aee1-3067af4d4edf%28Office.15%29.aspx) <br/> |Somente leitura  <br/> |
|[Isattachment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.isattachment%28v=exchg.80%29.aspx) <br/> |Não disponível  <br/> |Somente leitura  <br/> |
|[IsDirty](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceobject.isdirty%28v=exchg.80%29.aspx) <br/> |Não disponível  <br/> |Somente leitura  <br/> |
|[IsNew](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.isnew%28v=exchg.80%29.aspx) <br/> |Não disponível  <br/> |Somente leitura  <br/> |
|[Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceobject.item%28v=exchg.80%29.aspx) <br/> |[Item](https://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) <br/> |Somente leitura  <br/> |
|[MimeContent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) <br/> |[MimeContent](https://msdn.microsoft.com/library/4f472a08-5653-4c54-ba65-831dfe32f20f%28Office.15%29.aspx) <br/> |Somente leitura  <br/> |
|Não disponível  <br/> |[MimeContentUTF8](https://msdn.microsoft.com/library/31544c95-5231-4b57-958c-2a689464d29b%28Office.15%29.aspx) <br/> |Somente leitura  <br/> |
|[NormalizedBody](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.normalizedbody%28v=exchg.80%29.aspx) <br/> |[NormalizedBody](https://msdn.microsoft.com/library/bfb813e4-642d-4f1b-9e91-1fee89dbd083%28Office.15%29.aspx) <br/> |Somente leitura  <br/> |
|[PolicyTag](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.policytag%28v=exchg.80%29.aspx) <br/> |[PolicyTag](https://msdn.microsoft.com/library/fa4b1447-dc7b-47ad-a677-78fcee443dc6%28Office.15%29.aspx) <br/> |Leitura-gravação  <br/> |
|[Visualização](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.preview%28v=exchg.80%29.aspx) <br/> |[Visualização](https://msdn.microsoft.com/library/5d33f557-c9d5-4f7f-82c0-d800412f8b7e%28Office.15%29.aspx) <br/> |Leitura-gravação  <br/> |
|[RetentionDate](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.retentiondate%28v=exchg.80%29.aspx) <br/> |[RetentionDate](https://msdn.microsoft.com/library/0c1df5e2-b56a-4947-a047-2b73b32e5fb7%28Office.15%29.aspx) <br/> |Somente leitura  <br/> |
|[Esquema](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceobject.schema%28v=exchg.80%29.aspx) <br/> |Não disponível  <br/> |Somente leitura  <br/> |
|[Serviço](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceobject.service%28v=exchg.80%29.aspx) <br/> |Não disponível  <br/> |Somente leitura  <br/> |
|[StoreEntryId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.storeentryid%28v=exchg.80%29.aspx) <br/> |[StoreEntryId](https://msdn.microsoft.com/library/f536e264-8c4d-4cc5-bab8-22a4fa38de39%28Office.15%29.aspx) <br/> |Somente leitura  <br/> |
|[TextBody](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.textbody%28v=exchg.80%29.aspx) <br/> |[TextBody](https://msdn.microsoft.com/library/bd0c0bce-3e7c-47c7-af7f-5ee5f5ad9820%28Office.15%29.aspx) <br/> |Somente leitura  <br/> |
|[UniqueBody](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.uniquebody%28v=exchg.80%29.aspx) <br/> |[UniqueBody](https://msdn.microsoft.com/library/06bc95d7-121c-433b-bd27-c2b0eb8c011f%28Office.15%29.aspx) <br/> |Somente leitura  <br/> |
   
## <a name="see-also"></a>Confira também


- [Email e EWS no Exchange](email-and-ews-in-exchange.md)
    
- [Propriedades e propriedades estendidas no EWS no Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Conjuntos de propriedades e formas de resposta no EWS no Exchange](property-sets-and-response-shapes-in-ews-in-exchange.md)
    
- [Trabalhar com itens de caixa de correio do Exchange usando o EWS no Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)
    

