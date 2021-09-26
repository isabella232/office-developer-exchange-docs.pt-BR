---
title: Conjuntos de propriedades e formas de resposta no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 04a29804-6067-48e7-9f5c-534e253a230e
description: Aprenda a gerenciar as formas de resposta e os conjuntos de propriedades retornados pela API gerenciada EWS e pelo EWS Exchange.
ms.openlocfilehash: 7720a07a6fd288f289bba371ce6fd8a6e349a8ce
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543846"
---
# <a name="property-sets-and-response-shapes-in-ews-in-exchange"></a>Conjuntos de propriedades e formas de resposta no EWS no Exchange

Aprenda a gerenciar as formas de resposta e os conjuntos de propriedades retornados pela API gerenciada EWS e pelo EWS Exchange.
  
O Exchange de dados fornece uma solução de armazenamento flexível que permite armazenar itens diferentes, como contatos e entradas de calendário, na mesma pasta; no entanto, pode tornar difícil gerenciar os dados retornados de uma chamada para uma operação EWS ou um método de API gerenciada do EWS.
  
Para facilitar o gerenciamento dos dados retornados pelo Exchange Online, Exchange Online como parte do Office 365 ou versão do Excahange a partir do Exchange 2013, a API Gerenciada do EWS usa conjuntos de propriedades e o EWS usa formas de resposta. São coleções predefinidos que fornecem as propriedades mais comuns de um item de loja. O conjunto de propriedades retornadas é determinado pelo tipo de item. Isso significa que, ao vincular um item usando o método Exchange Managed API [Item.Bind,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) você obterá um conjunto diferente de propriedades, dependendo do tipo de item ao qual você se vincula. A associação a um item de calendário retornará um conjunto diferente de associação a um item de contato. Da mesma forma, se você estiver usando o EWS, a operação [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) retornará um conjunto diferente de propriedades com base no tipo de item retornado. 
  
A associação a uma pasta com o [método Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) ou o uso da operação [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) também retorna diferentes conjuntos de propriedades com base na pasta solicitada. 
  
**Tabela 1. Formas de resposta predefinida**

|**Forma de resposta**|**Equivalente à API Gerenciada do EWS**|**Descrição**|
|:-----|:-----|:-----|
|Somente ID  <br/> |[BasePropertySet.IdOnly](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) <br/> |Retorna apenas o identificador do item ou pasta. A maioria dos aplicativos deve usar essa forma de resposta e especificar as propriedades adicionais necessárias.  <br/> |
|Padrão  <br/> |N/A  <br/> |Retorna um conjunto predefinido de propriedades que são o padrão para o item ou pasta (somente EWS).  <br/> |
|Todas as propriedades  <br/> |[BasePropertySet.FirstClassProperties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) <br/> |Retorna as propriedades que os aplicativos cliente usam com mais frequência. Você pode retornar propriedades adicionais usando um caminho de propriedade.  <br/> |
   
## <a name="default-response-shapes"></a>Formas de resposta padrão

O EWS inclui um conjunto de formas de resposta padrão para pastas e itens. 
  
A tabela a seguir lista as propriedades padrão retornadas para cada pasta pelas operações [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) e [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) EWS. 
  
**Tabela 2. Propriedades de pasta padrão**

|**Propriedade**|**Caixa de Entrada**|**Calendar**|**Contacts**|**Itens excluídos**|**Rascunhos**|**Observações**|**Outras pastas**|**Caixa de saída**|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Nome de exibição  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|ID da pasta  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Contagem de subpastas  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Contagem total  <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Contagem não lida  <br/> |X  <br/> |||X  <br/> |X  <br/> ||X  <br/> |X  <br/> |
   
A tabela a seguir lista as propriedades padrão retornadas para cada tipo de item pelas operações [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) e [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS. 
  
**Tabela 3. Propriedades de item padrão**

|**Propriedade**|**Item de calendário**|**Item de Contato**|**Item de mensagem**|**Item de Tarefa**|
|:-----|:-----|:-----|:-----|:-----|
|Corpo  <br/> |||X(1)  <br/> ||
|CalendarItemType  <br/> ||x  <br/> |||
|CompanyName  <br/> ||x  <br/> |||
|CompleteName  <br/> ||x  <br/> |||
|DateTimeCreated  <br/> |||x  <br/> ||
|DateTimeSent  <br/> |||x  <br/> ||
|DueDate  <br/> ||||x(2)  <br/> |
|EmailAddresses  <br/> ||x  <br/> |||
|End  <br/> |x  <br/> ||||
|FileAs  <br/> ||x  <br/> |||
|De  <br/> |||x  <br/> ||
|HasAttachments  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ImAddresses  <br/> ||x  <br/> |||
|IsAssociated  <br/> |x  <br/> ||x  <br/> ||
|IsDeliveryReceiptRequested  <br/> |||x  <br/> ||
|ItemId  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|JobTitle  <br/> ||x  <br/> |||
|LegacyFreeBusyStatus  <br/> |x  <br/> ||||
|Local  <br/> |x  <br/> ||||
|Organizer  <br/> |x  <br/> ||||
|PercentComplete  <br/> ||||x  <br/> |
|PhoneNumbers  <br/> ||x  <br/> |||
|PhysicalAddresses  <br/> ||x  <br/> |||
|ResponseObjects  <br/> |x(1)  <br/> ||x(1)  <br/> ||
|Sensibilidade  <br/> |||x  <br/> ||
|Size  <br/> |||x  <br/> ||
|StartDate  <br/> ||||x(2)  <br/> |
|Status  <br/> ||||x  <br/> |
|Assunto  <br/> |x  <br/> ||x  <br/> |x  <br/> |
   
Observações:
  
1. Incluído na resposta da operação **GetItem.** Não incluído na resposta da operação **FindItem.** 
    
2. Somente incluído na resposta se o campo contiver dados. Não incluído na resposta se o campo estiver em branco.
    
### <a name="all-properties-set-and-response-shape"></a>Conjunto de propriedades e forma de resposta

A tabela a seguir lista as propriedades de primeira classe retornadas chamando os métodos de API Gerenciada [item.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) e [Item.FindItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) EWS Managed API e a forma de resposta "todas as propriedades" retornadas pelas operações [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) e [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS. 
  
Você pode adicionar propriedades adicionais ao conjunto de propriedades ou incluir propriedades estendidas. Para obter detalhes, consulte [Properties and extended properties in EWS in Exchange](properties-and-extended-properties-in-ews-in-exchange.md).
  
**Tabela 4. Propriedades de primeira classe**

|||||||
|:-----|:-----|:-----|:-----|:-----|:-----|
|Propriedade  <br/> |Item de calendário  <br/> |Item de Contato  <br/> |Item de mensagem  <br/> |Post item  <br/> |Item de Tarefa  <br/> |
|ActualWork  <br/> |||||x  <br/> |
|AdjacentMeetingCount  <br/> |x  <br/> |||||
|AdjacentMeetings  <br/> |x  <br/> |||||
|Alias  <br/> ||x  <br/> ||||
|AllowNewTimeProposal  <br/> |x  <br/> |||||
|AppointmentReplyTime  <br/> |x  <br/> |||||
|AppointmentSequenceNumber  <br/> |x  <br/> |||||
|AppointmentState  <br/> |x  <br/> |||||
|AssignedTime  <br/> |||||x  <br/> |
|AssistantName  <br/> ||x  <br/> ||||
|BccRecipients  <br/> |||x  <br/> |||
|BillingInformation  <br/> |||||x  <br/> |
|Corpo  <br/> |x(1)  <br/> |x(1)  <br/> |x(1)  <br/> ||x(1)  <br/> |
|BusinessHomePage  <br/> ||x  <br/> |x  <br/> |||
|CalendarItemType  <br/> |x  <br/> |||||
|Categories  <br/> |x  <br/> ||x  <br/> |x  <br/> |x  <br/> |
|CcRecipients  <br/> |||x  <br/> |||
|ChangeCount  <br/> |||||x  <br/> |
|Children  <br/> ||x  <br/> ||||
|Companies  <br/> |||||x  <br/> |
|CompleteDate  <br/> |||||x  <br/> |
|CompleteName  <br/> ||x  <br/> ||||
|ConferenceType  <br/> |x  <br/> |||||
|ConflictingMeetingCount  <br/> |x  <br/> |||||
|ConflictingMeetings  <br/> |x  <br/> |||||
|Contatos  <br/> |||||x  <br/> |
|ContactSource  <br/> ||x  <br/> ||||
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
|DirectoryId  <br/> ||x  <br/> ||||
|DirectReports  <br/> ||x  <br/> ||||
|DisplayCc  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DisplayName  <br/> ||x  <br/> ||||
|DisplayTo  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DueDate  <br/> |||||x  <br/> |
|Duração  <br/> |x  <br/> |||||
|EffectiveRights  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|EmailAddresses  <br/> ||x  <br/> ||||
|End  <br/> |x  <br/> |||||
|EndTimeZone  <br/> |x  <br/> |||||
|FileAs  <br/> ||x  <br/> ||||
|FileAsMapping  <br/> ||x  <br/> ||||
|FirstOccurrence  <br/> |x  <br/> |||||
|De  <br/> |||x  <br/> |x  <br/> ||
|Generation  <br/> ||x  <br/> ||||
|GivenName  <br/> ||x  <br/> ||||
|HasAttachments  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|HasPicture  <br/> ||x  <br/> ||||
|ImAddresses  <br/> ||x  <br/> ||||
|Importance  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Initials  <br/> ||x  <br/> ||||
|InReplyTo  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|InternetMessageId  <br/> |||x  <br/> |x  <br/> ||
|InternetMessageHeaders  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsAllDayEvent  <br/> |x  <br/> |||||
|IsAssociated  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsCancelled  <br/> |x  <br/> |||||
|IsComplete  <br/> |||||x  <br/> |
|IsDeliveryReceiptRequested  <br/> |||x  <br/> |||
|IsDraft  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsFromMe  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsMeeting  <br/> |x  <br/> |||||
|IsOnlineMeeting  <br/> |x  <br/> |||||
|IsRead  <br/> |||x  <br/> |||
|IsReadReceiptRequested  <br/> |||x  <br/> |||
|IsRecurring  <br/> |x  <br/> ||||x  <br/> |
|IsResend  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsResponseRequested  <br/> |x  <br/> ||x  <br/> |||
|IsSubmitted  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsUnmodified  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ItemClass  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ItemId  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|JobTitle  <br/> ||x  <br/> ||||
|LastModifiedName  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|LastModifiedTime  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|LastOccurrance  <br/> |x  <br/> |||||
|LegacyFreeBusyStatus  <br/> |x  <br/> |||||
|Local  <br/> |x  <br/> |||||
|Manager  <br/> ||x  <br/> ||||
|MeetingRequestWasSent  <br/> |x  <br/> |||||
|MeetingTimeZone  <br/> |x  <br/> |||||
|MeetingWorkspaceUrl  <br/> |x  <br/> |||||
|MiddleName  <br/> ||x  <br/> ||||
|Mileage  <br/> ||x  <br/> |||x  <br/> |
|ModifiedOccurrances  <br/> |x  <br/> |||||
|MyResponseType  <br/> |x  <br/> |||||
|NetShowUrl  <br/> |x  <br/> |||||
|NickName  <br/> ||x  <br/> ||||
|Observações  <br/> ||x  <br/> ||||
|OfficeLocation  <br/> ||x  <br/> ||||
|OptionalAttendees  <br/> |x  <br/> |||||
|Organizer  <br/> |x  <br/> |||||
|OriginalStart  <br/> |x  <br/> |||||
|Proprietário  <br/> |||||x  <br/> |
|ParentFolderId  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|PercentComplete  <br/> |||||x  <br/> |
|PhoneNumbers  <br/> ||x  <br/> ||||
|PhoneticFirstName  <br/> ||x  <br/> ||||
|PhoneticFullName  <br/> ||x  <br/> ||||
|PhoneticLastName  <br/> ||x  <br/> ||||
|Photo  <br/> ||x  <br/> ||||
|PhysicalAddresses  <br/> ||x  <br/> ||||
|PostalAddressIndex  <br/> ||x  <br/> ||||
|PostedTime  <br/> ||||x  <br/> ||
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
|ResponseObjects  <br/> |x(1)  <br/> |x(1)  <br/> |x(1)  <br/> |x(1)  <br/> |x(1)  <br/> |
|Remetente  <br/> |||x  <br/> |x  <br/> ||
|Sensitivity  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Size  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|SpouseName  <br/> ||x  <br/> ||||
|Início  <br/> |x  <br/> |||||
|StartDate  <br/> |||||x  <br/> |
|StartTimeZone  <br/> |x  <br/> |||||
|Status  <br/> |||||x  <br/> |
|StatusDescription  <br/> |||||x  <br/> |
|Assunto  <br/> |x  <br/> |x  <br/> |x  <br/> ||x  <br/> |
|Surname  <br/> ||x  <br/> ||||
|TimeZone  <br/> |x  <br/> |||||
|ToRecipients  <br/> |||x  <br/> |||
|TotalWork  <br/> |||||x  <br/> |
|WebClientEditFormQueryString  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|WebClientReadFormQueryString  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
   
Observações:
  
1. Incluído ao [vincular a um item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) e na resposta da [operação GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx). Não incluído no resultado do [método Item.FindItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou da resposta da [operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx).
    
## <a name="see-also"></a>Confira também

- [Desenvolver clientes do serviço Web para o Exchange](develop-web-service-clients-for-exchange.md)
    
- [Operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [Operação GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx)
    
- [Operação FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [Operação GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)
    

