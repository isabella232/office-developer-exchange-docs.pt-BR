---
title: RightsManagementLicenseData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 38f0b7f4-2338-4e90-af67-e0951e8edfa3
description: O elemento RightsManagementLicenseData especifica informações sobre a licença de gerenciamento de direitos de um item.
ms.openlocfilehash: 8875e9bad425224f86b6de5149f87a36c2a2581e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523465"
---
# <a name="rightsmanagementlicensedata"></a>RightsManagementLicenseData

O **elemento RightsManagementLicenseData** especifica informações sobre a licença de gerenciamento de direitos de um item. 
  
```XML
<RightsManagementLicenseData>
   <RightsManagedMessageDecryptionStatus/>
   <RmsTemplateId/>
   <TemplateName/>
   <TemplateDescription/>
   <EditAllowed/>
   <ReplyAllowed/>
   <ReplyAllAllowed/>
   <ForwardAllowed/>
   <ModifyRecipientsAllowed/>
   <ExtractAllowed/>
   <PrintAllowed/>
   <ExportAllowed/>
   <ProgrammaticAccessAllowed/>
   <IsOwner/>
   <ContentOwner/>
   <ContentExpiryDate/>
</RightsManagementLicenseData>
```

 **RightsManagementLicenseDataType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[RightsManagedMessageDecryptionStatus](rightsmanagedmessagedecryptionstatus.md)  |  [RMSTemplateId](rmstemplateid.md)  |  [TemplateName](templatename.md)  |  [TemplateDescription](templatedescription.md)  |  [EditAllowed](editallowed.md)  |  [ReplyAllowed](replyallowed.md)  |  [ReplyAllAllowed](replyallallowed.md)  |  [ForwardAllowed](forwardallowed.md)  |  [ModifyRecipientsAllowed](modifyrecipientsallowed.md)  |  [ExtractAllowed](extractallowed.md)  |  [PrintAllowed](printallowed.md)  |  [ExportAllowed](exportallowed.md)  |  [ProgrammaticAccessAllowed](programmaticaccessallowed.md)  |  [IsOwner](isowner.md)  |  [ContentOwner](contentowner.md)  |  [ContentExpiryDate](contentexpirydate.md)
  
### <a name="parent-elements"></a>Elementos pai

[Item](item.md)  |  [Mensagem](message-ex15websvcsotherref.md)  |  [MeetingMessage](meetingmessage.md)  |  [MeetingRequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [Tarefa](task.md)  |  [PostItem](postitem.md)  |  [CalendarItem](calendaritem.md)  |  [Contato](contact.md)  |  [DistributionList](distributionlist.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

