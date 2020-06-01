---
title: SearchPreviewItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 59b0b2db-a0ae-4162-a2cb-5f37f42fe872
description: O elemento SearchPreviewItem especifica a visualização do item para uma pesquisa de descoberta.
ms.openlocfilehash: ab48353b0ffaf4bc3b9409f1a620d145bffc7a13
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466931"
---
# <a name="searchpreviewitem"></a><span data-ttu-id="534ce-103">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="534ce-103">SearchPreviewItem</span></span>

<span data-ttu-id="534ce-104">O elemento **SearchPreviewItem** especifica a visualização do item para uma pesquisa de descoberta.</span><span class="sxs-lookup"><span data-stu-id="534ce-104">The **SearchPreviewItem** element specifies the item preview for a discovery search.</span></span> 
  
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

 <span data-ttu-id="534ce-105">**SearchPreviewItemType**</span><span class="sxs-lookup"><span data-stu-id="534ce-105">**SearchPreviewItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="534ce-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="534ce-106">Attributes and elements</span></span>

<span data-ttu-id="534ce-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="534ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="534ce-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="534ce-108">Attributes</span></span>

<span data-ttu-id="534ce-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="534ce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="534ce-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="534ce-110">Child elements</span></span>

<span data-ttu-id="534ce-111">[ID (ItemIdType)](id-itemidtype.md)  |  [Caixa de correio (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md)  |  [ParentID](parentid.md)  |  @ [Class](itemclass.md)  |  [UniqueHash](uniquehash.md)  |  [Sortvalue](sortvalue.md)  |  [OwaLink](owalink.md)  |  [Remetente (cadeia de caracteres)](sender-string.md)  |  [ToRecipients (ArrayOfSmtpAddressType)](torecipients-arrayofsmtpaddresstype.md)  |  [CcRecipients](ccrecipients.md)  |  [BccRecipients](bccrecipients.md)  |  [Createdtime](createdtime.md)  |  [Receivedtime](receivedtime.md)  |  [SentTime](senttime.md)  |  [Assunto](subject.md)  |  [Tamanho (longo)](size-long.md)  |  [Visualização](preview-ex15websvcsotherref.md)  |  [Importância](importance.md)  |  [Ler](read.md)  |  [HasAttachment](hasattachment.md)  |  [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)</span><span class="sxs-lookup"><span data-stu-id="534ce-111">[ID (ItemIdType)](id-itemidtype.md) | [Mailbox (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md) | [ParentId](parentid.md) | [ItemClass](itemclass.md) | [UniqueHash](uniquehash.md) | [SortValue](sortvalue.md) | [OwaLink](owalink.md) | [Sender (string)](sender-string.md) | [ToRecipients (ArrayOfSmtpAddressType)](torecipients-arrayofsmtpaddresstype.md) | [CcRecipients](ccrecipients.md) | [BccRecipients](bccrecipients.md) | [CreatedTime](createdtime.md) | [ReceivedTime](receivedtime.md) | [SentTime](senttime.md) | [Subject](subject.md) | [Size (long)](size-long.md) | [Preview](preview-ex15websvcsotherref.md) | [Importance](importance.md) | [Read](read.md) | [HasAttachment](hasattachment.md) | [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="534ce-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="534ce-112">Parent elements</span></span>

[<span data-ttu-id="534ce-113">Itens (ArrayOfSearchPreviewItemsType)</span><span class="sxs-lookup"><span data-stu-id="534ce-113">Items (ArrayOfSearchPreviewItemsType)</span></span>](items-arrayofsearchpreviewitemstype.md)
  
## <a name="remarks"></a><span data-ttu-id="534ce-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="534ce-114">Remarks</span></span>

<span data-ttu-id="534ce-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="534ce-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="534ce-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="534ce-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="534ce-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="534ce-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="534ce-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="534ce-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="534ce-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="534ce-119">Schema name</span></span>  <br/> |<span data-ttu-id="534ce-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="534ce-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="534ce-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="534ce-121">Validation file</span></span>  <br/> |<span data-ttu-id="534ce-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="534ce-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="534ce-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="534ce-123">Can be empty</span></span>  <br/> ||
   

