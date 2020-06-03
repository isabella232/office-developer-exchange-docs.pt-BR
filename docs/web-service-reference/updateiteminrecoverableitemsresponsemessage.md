---
title: UpdateItemInRecoverableItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96259756-322e-4c24-ac76-0cd9c32e0d6d
description: O elemento UpdateItemInRecoverableItemsResponseMessage especifica a resposta a uma solicitação UpdateItemInRecoverableItems.
ms.openlocfilehash: 021631f5c30eebbf4d7ae0aad35a85b99a23925f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466532"
---
# <a name="updateiteminrecoverableitemsresponsemessage"></a><span data-ttu-id="bab9c-103">UpdateItemInRecoverableItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bab9c-103">UpdateItemInRecoverableItemsResponseMessage</span></span>

<span data-ttu-id="bab9c-104">O elemento **UpdateItemInRecoverableItemsResponseMessage** especifica a resposta a uma solicitação **UpdateItemInRecoverableItems** .</span><span class="sxs-lookup"><span data-stu-id="bab9c-104">The **UpdateItemInRecoverableItemsResponseMessage** element specifies the response to an **UpdateItemInRecoverableItems** request.</span></span> 
  
```XML
<UpdateItemInRecoverableItemsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKet/>
   <MessageXml/>
   <Items/>
   <Attachments/>
   <ConflictResults/>
</UpdateItemInRecoverableItemsResponseMessage>
```

 <span data-ttu-id="bab9c-105">**UpdateItemInRecoverableItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="bab9c-105">**UpdateItemInRecoverableItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bab9c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="bab9c-106">Attributes and elements</span></span>

<span data-ttu-id="bab9c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bab9c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bab9c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="bab9c-108">Attributes</span></span>

<span data-ttu-id="bab9c-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bab9c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bab9c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bab9c-110">Child elements</span></span>

<span data-ttu-id="bab9c-111">[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [DescriptiveLinkKey](descriptivelinkkey.md)  |  [MessageXml](messagexml.md)  |  [Itens](items.md)  |  [Anexos](attachments-ex15websvcsotherref.md)  |  [ConflictResults](conflictresults.md)</span><span class="sxs-lookup"><span data-stu-id="bab9c-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [Items](items.md) | [Attachments](attachments-ex15websvcsotherref.md) | [ConflictResults](conflictresults.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bab9c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bab9c-112">Parent elements</span></span>

<span data-ttu-id="bab9c-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bab9c-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bab9c-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="bab9c-114">Remarks</span></span>

<span data-ttu-id="bab9c-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bab9c-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bab9c-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="bab9c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bab9c-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="bab9c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bab9c-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="bab9c-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|<span data-ttu-id="bab9c-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="bab9c-119">Schema name</span></span>  <br/> |<span data-ttu-id="bab9c-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="bab9c-120">Message schema</span></span>  <br/> |
|<span data-ttu-id="bab9c-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="bab9c-121">Validation file</span></span>  <br/> |<span data-ttu-id="bab9c-122">Message. xsd</span><span class="sxs-lookup"><span data-stu-id="bab9c-122">Message.xsd</span></span>  <br/> |
|<span data-ttu-id="bab9c-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="bab9c-123">Can be empty</span></span>  <br/> |<span data-ttu-id="bab9c-124">falso</span><span class="sxs-lookup"><span data-stu-id="bab9c-124">false</span></span>  <br/> |
   

