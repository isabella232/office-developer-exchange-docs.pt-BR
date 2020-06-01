---
title: Conjuntos de propriedades e formas de resposta no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 04a29804-6067-48e7-9f5c-534e253a230e
description: Saiba como gerenciar as formas de resposta e os conjuntos de propriedades que são retornados pela API gerenciada do EWS e pelo EWS no Exchange.
ms.openlocfilehash: 8f539a2131798e764574ef92f75deb654c02c90f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457659"
---
# <a name="property-sets-and-response-shapes-in-ews-in-exchange"></a>Conjuntos de propriedades e formas de resposta no EWS no Exchange

Saiba como gerenciar as formas de resposta e os conjuntos de propriedades que são retornados pela API gerenciada do EWS e pelo EWS no Exchange.
  
O repositório de dados do Exchange oferece uma solução de armazenamento flexível que permite armazenar itens diferentes, como contatos e entradas de calendário, na mesma pasta; no entanto, pode dificultar o gerenciamento dos dados retornados de uma chamada para uma operação do EWS ou um método de API gerenciada do EWS.
  
Para facilitar o gerenciamento dos dados retornados pelo Exchange Online, do Exchange Online como parte do Office 365, ou da versão do excahange a partir do Exchange 2013, a API gerenciada do EWS usa conjuntos de propriedades e o EWS usa formas de resposta. São coleções predefinidas que fornecem as propriedades mais comuns de um item de armazenamento. O conjunto de propriedades que é retornado é determinado pelo tipo de item. Isso significa que, quando você vincula um item usando o item Exchange Managed API [. método BIND](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) , você obtém um conjunto de propriedades diferente dependendo do tipo de item para o qual você vincular. A associação a um item de calendário retornará um conjunto diferente de propriedades do que a associação a um item de contato. Da mesma forma, se você estiver usando o EWS, a [operação GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) retornará um conjunto diferente de propriedades com base no tipo de item que é retornado. 
  
A associação a uma pasta com o método [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) ou usando a [operação GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) também retorna conjuntos diferentes de propriedades com base na pasta solicitada. 
  
**Tabela 1. Formas de resposta predefinidas**

|**Forma de resposta**|**Equivalente à API gerenciada do EWS**|**Descrição**|
|:-----|:-----|:-----|
|Somente ID  <br/> |[BasePropertySet.IdOnly](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) <br/> |Retorna somente o identificador do item ou pasta. A maioria dos aplicativos deve usar essa forma de resposta e especificar quaisquer propriedades adicionais necessárias.  <br/> |
|Padrão  <br/> |N/A  <br/> |Retorna um conjunto predefinido de propriedades que são o padrão para o item ou pasta (somente EWS).  <br/> |
|Todas as propriedades  <br/> |[BasePropertySet.FirstClassProperties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) <br/> |Retorna as propriedades que os aplicativos clientes usam com mais frequência. Você pode retornar propriedades adicionais usando um caminho de propriedade.  <br/> |
   
## <a name="default-response-shapes"></a>Formas de resposta padrão

O EWS inclui um conjunto de formas de resposta padrão para pastas e itens. 
  
A tabela a seguir lista as propriedades padrão que são retornadas para cada pasta pelas operações [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) e [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) EWS. 
  
**Tabela 2. Propriedades da pasta padrão**

|**Propriedade**|**Caixa de Entrada**|**Calendar**|**Contacts**|**Itens excluídos**|**Rascunhos**|**Anotações**|**Outras pastas**|**Enviada**|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Nome diferenciado (DN)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|ID da pasta  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Contagem de subpastas  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Contagem total  <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Contagem de não lidos  <br/> |X  <br/> |||X  <br/> |X  <br/> ||X  <br/> |X  <br/> |
   
A tabela a seguir lista as propriedades padrão que são retornadas para cada tipo de item pelas operações do EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) e [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) . 
  
**Tabela 3. Propriedades de item padrão**

|**Propriedade**|**Item de calendário**|**Item de Contato**|**Item de mensagem**|**Item de Tarefa**|
|:-----|:-----|:-----|:-----|:-----|
|Corpo  <br/> |||X (1)  <br/> ||
|CalendarItemType  <br/> ||x  <br/> |||
|CompanyName  <br/> ||x  <br/> |||
|CompleteName  <br/> ||x  <br/> |||
|DateTimeCreated  <br/> |||x  <br/> ||
|DateTimeSent  <br/> |||x  <br/> ||
|Data de Conclusão  <br/> ||||x (2)  <br/> |
|EndereçosEmail  <br/> ||x  <br/> |||
|Final  <br/> |x  <br/> ||||
|FileAs  <br/> ||x  <br/> |||
|From  <br/> |||x  <br/> ||
|HasAttachments  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Imendereços  <br/> ||x  <br/> |||
|Isassociated  <br/> |x  <br/> ||x  <br/> ||
|IsDeliveryReceiptRequested  <br/> |||x  <br/> ||
|ItemId  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|JobTitle  <br/> ||x  <br/> |||
|LegacyFreeBusyStatus  <br/> |x  <br/> ||||
|Local  <br/> |x  <br/> ||||
|Organizador  <br/> |x  <br/> ||||
|PercentComplete  <br/> ||||x  <br/> |
|PhoneNumbers  <br/> ||x  <br/> |||
|PhysicalAddresses  <br/> ||x  <br/> |||
|ResponseObjects  <br/> |x (1)  <br/> ||x (1)  <br/> ||
|Sensitity  <br/> |||x  <br/> ||
|Tamanho  <br/> |||x  <br/> ||
|StartDate  <br/> ||||x (2)  <br/> |
|Status  <br/> ||||x  <br/> |
|Assunto  <br/> |x  <br/> ||x  <br/> |x  <br/> |
   
Observações:
  
1. Incluído na resposta da operação **GetItem** . Não incluído na resposta da operação **FindItem** . 
    
2. Incluído apenas na resposta se o campo contiver dados. Não incluído na resposta se o campo estiver em branco.
    
### <a name="all-properties-set-and-response-shape"></a>Definição de todas as propriedades e forma de resposta

A tabela a seguir lista as propriedades de primeira classe que são retornadas chamando-se o item de API gerenciada do EWS [. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) e [Item. FindItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) os métodos da API gerenciada do EWS e a forma de resposta "todas as propriedades" retornadas pelas operações do EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) e do [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) . 
  
Você pode adicionar propriedades adicionais ao conjunto de propriedades ou incluir propriedades estendidas. Para obter detalhes, consulte [Propriedades e propriedades estendidas no EWS no Exchange](properties-and-extended-properties-in-ews-in-exchange.md).
  
**Tabela 4. Propriedades de primeira classe**

|||||||
|:-----|:-----|:-----|:-----|:-----|:-----|
|Propriedade  <br/> |Item de calendário  <br/> |Item de Contato  <br/> |Item de mensagem  <br/> |Item de postagem  <br/> |Item de Tarefa  <br/> |
|ActualWork  <br/> |||||x  <br/> |
|AdjacentMeetingCount  <br/> |x  <br/> |||||
|AdjacentMeetings  <br/> |x  <br/> |||||
|Alias  <br/> ||x  <br/> ||||
|AllowNewTimeProposal  <br/> |x  <br/> |||||
|AppointmentReplyTime  <br/> |x  <br/> |||||
|AppointmentSequenceNumber  <br/> |x  <br/> |||||
|Compromissostate  <br/> |x  <br/> |||||
|AssignedTime  <br/> |||||x  <br/> |
|AssistantName  <br/> ||x  <br/> ||||
|BccRecipients  <br/> |||x  <br/> |||
|BillingInformation  <br/> |||||x  <br/> |
|Corpo  <br/> |x (1)  <br/> |x (1)  <br/> |x (1)  <br/> ||x (1)  <br/> |
|BusinessHomePage  <br/> ||x  <br/> |x  <br/> |||
|CalendarItemType  <br/> |x  <br/> |||||
|Categorias  <br/> |x  <br/> ||x  <br/> |x  <br/> |x  <br/> |
|CcRecipients  <br/> |||x  <br/> |||
|ChangeCount  <br/> |||||x  <br/> |
|Crianças  <br/> ||x  <br/> ||||
|Empresas  <br/> |||||x  <br/> |
|Concluído  <br/> |||||x  <br/> |
|CompleteName  <br/> ||x  <br/> ||||
|ConferenceType  <br/> |x  <br/> |||||
|ConflictingMeetingCount  <br/> |x  <br/> |||||
|ConflictingMeetings  <br/> |x  <br/> |||||
|Contatos  <br/> |||||x  <br/> |
|Contato  <br/> ||x  <br/> ||||
|ConversationId  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ConversationIndex  <br/> |||x  <br/> |x  <br/> ||
|ConversationTopic  <br/> |||x  <br/> |x  <br/> ||
|Cultura  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DateTimeCreated  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DateTimeReceived  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DateTimeSent  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DateTimeStamp  <br/> |x  <br/> |||||
|DelegationState  <br/> |||||x  <br/> |
|Delegator  <br/> |||||x  <br/> |
|DeletedOccurrences  <br/> |x  <br/> |||||
|Departamento  <br/> ||x  <br/> ||||
|Directoryid  <br/> ||x  <br/> ||||
|DirectReports  <br/> ||x  <br/> ||||
|DisplayCc  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DisplayName  <br/> ||x  <br/> ||||
|DisplayTo  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Data de Conclusão  <br/> |||||x  <br/> |
|Duração  <br/> |x  <br/> |||||
|EffectiveRights  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|EndereçosEmail  <br/> ||x  <br/> ||||
|Final  <br/> |x  <br/> |||||
|EndTimeZone  <br/> |x  <br/> |||||
|FileAs  <br/> ||x  <br/> ||||
|FileAsMapping  <br/> ||x  <br/> ||||
|FirstOccurrence  <br/> |x  <br/> |||||
|From  <br/> |||x  <br/> |x  <br/> ||
|Várias  <br/> ||x  <br/> ||||
|GivenName  <br/> ||x  <br/> ||||
|HasAttachments  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|HasPicture  <br/> ||x  <br/> ||||
|Imendereços  <br/> ||x  <br/> ||||
|Importance  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Iniciais  <br/> ||x  <br/> ||||
|Inresponderto  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|InternetMessageId  <br/> |||x  <br/> |x  <br/> ||
|Propriedadeinternetmessageheaders  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsAllDayEvent  <br/> |x  <br/> |||||
|Isassociated  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsCanceled  <br/> |x  <br/> |||||
|IsComplete  <br/> |||||x  <br/> |
|IsDeliveryReceiptRequested  <br/> |||x  <br/> |||
|IsDraft  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsFromMe  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Issatisfaçing  <br/> |x  <br/> |||||
|IsOnlineMeeting  <br/> |x  <br/> |||||
|IsRead  <br/> |||x  <br/> |||
|IsReadReceiptRequested  <br/> |||x  <br/> |||
|IsRecurring  <br/> |x  <br/> ||||x  <br/> |
|IsResend  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsResponseRequested  <br/> |x  <br/> ||x  <br/> |||
|Isenviado  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsUnmodified  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ItemClass  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ItemId  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|JobTitle  <br/> ||x  <br/> ||||
|LastModified  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|LastModifiedTime  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|LastOccurrance  <br/> |x  <br/> |||||
|LegacyFreeBusyStatus  <br/> |x  <br/> |||||
|Local  <br/> |x  <br/> |||||
|Gerente  <br/> ||x  <br/> ||||
|MeetingRequestWasSent  <br/> |x  <br/> |||||
|MeetingTimeZone  <br/> |x  <br/> |||||
|MeetingWorkspaceUrl  <br/> |x  <br/> |||||
|MiddleName  <br/> ||x  <br/> ||||
|Quilometragem  <br/> ||x  <br/> |||x  <br/> |
|ModifiedOccurrances  <br/> |x  <br/> |||||
|MyResponseType  <br/> |x  <br/> |||||
|NetShowUrl  <br/> |x  <br/> |||||
|NickName  <br/> ||x  <br/> ||||
|Observações  <br/> ||x  <br/> ||||
|OfficeLocation  <br/> ||x  <br/> ||||
|OptionalAttendees  <br/> |x  <br/> |||||
|Organizador  <br/> |x  <br/> |||||
|OriginalStart  <br/> |x  <br/> |||||
|Proprietário  <br/> |||||x  <br/> |
|ParentFolderId  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|PercentComplete  <br/> |||||x  <br/> |
|PhoneNumbers  <br/> ||x  <br/> ||||
|PhoneticFirstName  <br/> ||x  <br/> ||||
|PhoneticFullName  <br/> ||x  <br/> ||||
|PhoneticLastName  <br/> ||x  <br/> ||||
|Foto  <br/> ||x  <br/> ||||
|PhysicalAddresses  <br/> ||x  <br/> ||||
|PostalAddressIndex  <br/> ||x  <br/> ||||
|Postadotime  <br/> ||||x  <br/> ||
|Profession  <br/> ||x  <br/> ||||
|ReceivedBy  <br/> |||x  <br/> |||
|ReceivedRepresenting  <br/> |||x  <br/> |||
|Reccurrence  <br/> |x  <br/> ||||x  <br/> |
|Referências  <br/> |||x  <br/> |x  <br/> ||
|ReminderDueBy  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ReminderIsSet  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ReminderMinutesBeforeStart  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ReplyTo  <br/> |||x  <br/> |||
|RequiredAttendees  <br/> |x  <br/> |||||
|Recursos  <br/> |x  <br/> |||||
|ResponseObjects  <br/> |x (1)  <br/> |x (1)  <br/> |x (1)  <br/> |x (1)  <br/> |x (1)  <br/> |
|Remetente  <br/> |||x  <br/> |x  <br/> ||
|Confidencialidade  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Tamanho  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Maridoname  <br/> ||x  <br/> ||||
|Início  <br/> |x  <br/> |||||
|StartDate  <br/> |||||x  <br/> |
|StartTimeZone  <br/> |x  <br/> |||||
|Status  <br/> |||||x  <br/> |
|StatusDescription  <br/> |||||x  <br/> |
|Assunto  <br/> |x  <br/> |x  <br/> |x  <br/> ||x  <br/> |
|Sobrenome  <br/> ||x  <br/> ||||
|TimeZone  <br/> |x  <br/> |||||
|ToRecipients  <br/> |||x  <br/> |||
|TotalWork  <br/> |||||x  <br/> |
|WebClientEditFormQueryString  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|WebClientReadFormQueryString  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
   
Observações:
  
1. Incluído na [associação a um item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) e na resposta da [operação GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx). Não incluído no resultado do método [Item. FindItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou a resposta da [operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx).
    
## <a name="see-also"></a>Também consulte

- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [Operação GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx)
    
- [Operação FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [Operação GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)
    

