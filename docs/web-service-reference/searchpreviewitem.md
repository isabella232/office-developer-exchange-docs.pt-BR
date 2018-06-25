---
title: SearchPreviewItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 59b0b2db-a0ae-4162-a2cb-5f37f42fe872
description: O elemento SearchPreviewItem Especifica a visualização de item de uma pesquisa de descoberta.
ms.openlocfilehash: 46b9d6049f856ce6e93b9e49e07516ec4b52d932
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825308"
---
# <a name="searchpreviewitem"></a><span data-ttu-id="e0a1e-103">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="e0a1e-103">SearchPreviewItem</span></span>

<span data-ttu-id="e0a1e-104">O elemento **SearchPreviewItem** Especifica a visualização de item de uma pesquisa de descoberta.</span><span class="sxs-lookup"><span data-stu-id="e0a1e-104">The **SearchPreviewItem** element specifies the item preview for a discovery search.</span></span> 
  
```XML
<SearchPreviewItem>
   <Id/>
   <Mailbox/>
   <ParentId/>
   <ItemClass/>
   <UniqueHash/>
   <SortValue/>
   <OwaLink/>
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <CreatedTime/>
   <ReceivedTime/>
   <SentTime/>
   <Subject/>
   <Size/>
   <Preview/>
   <Importance/>
   <Read/>
   <HasAttachment/>
   <ExtendedProperties/>
</SearchPreviewItem>
```

 <span data-ttu-id="e0a1e-105">**SearchPreviewItemType**</span><span class="sxs-lookup"><span data-stu-id="e0a1e-105">**SearchPreviewItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e0a1e-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e0a1e-106">Attributes and elements</span></span>

<span data-ttu-id="e0a1e-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e0a1e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e0a1e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e0a1e-108">Attributes</span></span>

<span data-ttu-id="e0a1e-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e0a1e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e0a1e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e0a1e-110">Child elements</span></span>

<span data-ttu-id="e0a1e-111">[ID (ItemIdType)](id-itemidtype.md) | [caixa de correio (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md) | [ParentId](parentid.md) | [ItemClass](itemclass.md) | [UniqueHash](uniquehash.md) | [SortValue](sortvalue.md) | [OwaLink](owalink.md)  |  [ O remetente (string)](sender-string.md) | [ToRecipients (ArrayOfSmtpAddressType)](torecipients-arrayofsmtpaddresstype.md) | [CcRecipients](ccrecipients.md) | [BccRecipients](bccrecipients.md) | [CreatedTime](createdtime.md) | [ReceivedTime](receivedtime.md)  |  [Hora de envio](senttime.md)  |  [Assunto](subject.md) | [tamanho (long)](size-long.md) | [visualização](preview-ex15websvcsotherref.md) | [importância](importance.md) | [leitura](read.md) | [HasAttachment](hasattachment.md) | [(ExtendedProperties NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)</span><span class="sxs-lookup"><span data-stu-id="e0a1e-111">[ID (ItemIdType)](id-itemidtype.md) | [Mailbox (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md) | [ParentId](parentid.md) | [ItemClass](itemclass.md) | [UniqueHash](uniquehash.md) | [SortValue](sortvalue.md) | [OwaLink](owalink.md) | [Sender (string)](sender-string.md) | [ToRecipients (ArrayOfSmtpAddressType)](torecipients-arrayofsmtpaddresstype.md) | [CcRecipients](ccrecipients.md) | [BccRecipients](bccrecipients.md) | [CreatedTime](createdtime.md) | [ReceivedTime](receivedtime.md) | [SentTime](senttime.md) | [Subject](subject.md) | [Size (long)](size-long.md) | [Preview](preview-ex15websvcsotherref.md) | [Importance](importance.md) | [Read](read.md) | [HasAttachment](hasattachment.md) | [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e0a1e-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e0a1e-112">Parent elements</span></span>

[<span data-ttu-id="e0a1e-113">Itens (ArrayOfSearchPreviewItemsType)</span><span class="sxs-lookup"><span data-stu-id="e0a1e-113">Items (ArrayOfSearchPreviewItemsType)</span></span>](items-arrayofsearchpreviewitemstype.md)
  
## <a name="remarks"></a><span data-ttu-id="e0a1e-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="e0a1e-114">Remarks</span></span>

<span data-ttu-id="e0a1e-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e0a1e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e0a1e-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e0a1e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e0a1e-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e0a1e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e0a1e-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="e0a1e-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e0a1e-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e0a1e-119">Schema name</span></span>  <br/> |<span data-ttu-id="e0a1e-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e0a1e-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="e0a1e-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e0a1e-121">Validation file</span></span>  <br/> |<span data-ttu-id="e0a1e-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e0a1e-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e0a1e-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e0a1e-123">Can be empty</span></span>  <br/> ||
   

