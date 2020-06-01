---
title: MarkAsJunkResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3e2b7b53-ef3c-438e-93df-b08409dbab46
description: O elemento MarkAsJunkResponseMessage especifica a mensagem de resposta para uma solicitação MarkAsJunk.
ms.openlocfilehash: be03fc964b56c463320f09e68d143a0377300f5c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460096"
---
# <a name="markasjunkresponsemessage"></a><span data-ttu-id="4ce0e-103">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4ce0e-103">MarkAsJunkResponseMessage</span></span>

<span data-ttu-id="4ce0e-104">O elemento **MarkAsJunkResponseMessage** especifica a mensagem de resposta para uma solicitação **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="4ce0e-104">The **MarkAsJunkResponseMessage** element specifies the response message for a **MarkAsJunk** request.</span></span> 
  
```XML
<MarkAsJunkResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MovedItemId/>
</MarkAsJunkResponseMessage>
```

 <span data-ttu-id="4ce0e-105">**MarkAsJunkResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="4ce0e-105">**MarkAsJunkResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ce0e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4ce0e-106">Attributes and elements</span></span>

<span data-ttu-id="4ce0e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4ce0e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ce0e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4ce0e-108">Attributes</span></span>

<span data-ttu-id="4ce0e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ce0e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ce0e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4ce0e-110">Child elements</span></span>

<span data-ttu-id="4ce0e-111">[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [DescriptiveLinkKey](descriptivelinkkey.md)  |  [MessageXml](messagexml.md)  |  [MovedItemId](moveditemid.md)</span><span class="sxs-lookup"><span data-stu-id="4ce0e-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MovedItemId](moveditemid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4ce0e-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4ce0e-112">Parent elements</span></span>

[<span data-ttu-id="4ce0e-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4ce0e-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="4ce0e-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="4ce0e-114">Remarks</span></span>

<span data-ttu-id="4ce0e-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4ce0e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4ce0e-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ce0e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ce0e-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4ce0e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ce0e-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="4ce0e-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4ce0e-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4ce0e-119">Schema name</span></span>  <br/> |<span data-ttu-id="4ce0e-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="4ce0e-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4ce0e-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4ce0e-121">Validation file</span></span>  <br/> |<span data-ttu-id="4ce0e-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4ce0e-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4ce0e-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="4ce0e-123">Can be empty</span></span>  <br/> ||
   

