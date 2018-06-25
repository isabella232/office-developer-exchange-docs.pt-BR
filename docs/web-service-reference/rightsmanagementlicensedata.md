---
title: RightsManagementLicenseData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 38f0b7f4-2338-4e90-af67-e0951e8edfa3
description: O elemento RightsManagementLicenseData Especifica informações sobre a licença de gerenciamento de direitos para um item.
ms.openlocfilehash: ec2ba1dc155afe239c499246095f86fc621910a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825234"
---
# <a name="rightsmanagementlicensedata"></a><span data-ttu-id="1f872-103">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="1f872-103">RightsManagementLicenseData</span></span>

<span data-ttu-id="1f872-104">O elemento **RightsManagementLicenseData** Especifica informações sobre a licença de gerenciamento de direitos para um item.</span><span class="sxs-lookup"><span data-stu-id="1f872-104">The **RightsManagementLicenseData** element specifies information about the rights management license for an item.</span></span> 
  
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

 <span data-ttu-id="1f872-105">**RightsManagementLicenseDataType**</span><span class="sxs-lookup"><span data-stu-id="1f872-105">**RightsManagementLicenseDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f872-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1f872-106">Attributes and elements</span></span>

<span data-ttu-id="1f872-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1f872-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f872-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1f872-108">Attributes</span></span>

<span data-ttu-id="1f872-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1f872-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f872-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1f872-110">Child elements</span></span>

<span data-ttu-id="1f872-111">[RightsManagedMessageDecryptionStatus](rightsmanagedmessagedecryptionstatus.md) | [RMSTemplateId](rmstemplateid.md) | [TemplateName](templatename.md) | [TemplateDescription](templatedescription.md) | [EditAllowed](editallowed.md) | [ReplyAllowed](replyallowed.md)  |  [ ReplyAllAllowed](replyallallowed.md) | [ForwardAllowed](forwardallowed.md) | [ModifyRecipientsAllowed](modifyrecipientsallowed.md) | [ExtractAllowed](extractallowed.md) | [PrintAllowed](printallowed.md) | [ExportAllowed](exportallowed.md)  |  [ ProgrammaticAccessAllowed](programmaticaccessallowed.md) | [IsOwner](isowner.md) | [ContentOwner](contentowner.md) | [ContentExpiryDate](contentexpirydate.md)</span><span class="sxs-lookup"><span data-stu-id="1f872-111">[RightsManagedMessageDecryptionStatus](rightsmanagedmessagedecryptionstatus.md) | [RMSTemplateId](rmstemplateid.md) | [TemplateName](templatename.md) | [TemplateDescription](templatedescription.md) | [EditAllowed](editallowed.md) | [ReplyAllowed](replyallowed.md) | [ReplyAllAllowed](replyallallowed.md) | [ForwardAllowed](forwardallowed.md) | [ModifyRecipientsAllowed](modifyrecipientsallowed.md) | [ExtractAllowed](extractallowed.md) | [PrintAllowed](printallowed.md) | [ExportAllowed](exportallowed.md) | [ProgrammaticAccessAllowed](programmaticaccessallowed.md) | [IsOwner](isowner.md) | [ContentOwner](contentowner.md) | [ContentExpiryDate](contentexpirydate.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1f872-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1f872-112">Parent elements</span></span>

<span data-ttu-id="1f872-113">[Item](item.md) | [mensagem](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [tarefa](task.md) | [PostItem ](postitem.md)  |  [CalendarItem](calendaritem.md) | [contato](contact.md) | [DistributionList](distributionlist.md)</span><span class="sxs-lookup"><span data-stu-id="1f872-113">[Item](item.md) | [Message](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [Task](task.md) | [PostItem](postitem.md) | [CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1f872-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="1f872-114">Remarks</span></span>

<span data-ttu-id="1f872-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1f872-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1f872-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1f872-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f872-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="1f872-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f872-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="1f872-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1f872-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1f872-119">Schema name</span></span>  <br/> |<span data-ttu-id="1f872-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="1f872-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="1f872-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1f872-121">Validation file</span></span>  <br/> |<span data-ttu-id="1f872-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1f872-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1f872-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="1f872-123">Can be empty</span></span>  <br/> ||
   

