---
title: GetNonIndexableItemDetailsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00566965-6cbd-4f31-9fa9-85b3e5559c0c
description: O elemento GetNonIndexableItemDetailsResponseMessage especifica a mensagem de resposta para uma solicitação GetNonIndexableItemDetails.
ms.openlocfilehash: 4cf6b422cc29b20b09d05ea45628fa7133b437b2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456518"
---
# <a name="getnonindexableitemdetailsresponsemessage"></a><span data-ttu-id="9f9b7-103">GetNonIndexableItemDetailsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9f9b7-103">GetNonIndexableItemDetailsResponseMessage</span></span>

<span data-ttu-id="9f9b7-104">O elemento **GetNonIndexableItemDetailsResponseMessage** especifica a mensagem de resposta para uma solicitação **GetNonIndexableItemDetails** .</span><span class="sxs-lookup"><span data-stu-id="9f9b7-104">The **GetNonIndexableItemDetailsResponseMessage** element specifies the response message for a **GetNonIndexableItemDetails** request.</span></span> 
  
```XML
<GetNonIndexableItemDetailsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <NonIndexableItemDetailsResult/>
</GetNonIndexableItemDetailsResponseMessage>
```

 <span data-ttu-id="9f9b7-105">**GetNonIndexableItemDetailsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="9f9b7-105">**GetNonIndexableItemDetailsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f9b7-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9f9b7-106">Attributes and elements</span></span>

<span data-ttu-id="9f9b7-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9f9b7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f9b7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9f9b7-108">Attributes</span></span>

<span data-ttu-id="9f9b7-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9f9b7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f9b7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9f9b7-110">Child elements</span></span>

<span data-ttu-id="9f9b7-111">[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [DescriptiveLinkKey](descriptivelinkkey.md)  |  [MessageXml](messagexml.md)  |  [NonIndexableItemDetailsResult](nonindexableitemdetailsresult.md)</span><span class="sxs-lookup"><span data-stu-id="9f9b7-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [NonIndexableItemDetailsResult](nonindexableitemdetailsresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9f9b7-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9f9b7-112">Parent elements</span></span>

[<span data-ttu-id="9f9b7-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9f9b7-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="9f9b7-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="9f9b7-114">Remarks</span></span>

<span data-ttu-id="9f9b7-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9f9b7-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9f9b7-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9f9b7-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f9b7-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9f9b7-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f9b7-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="9f9b7-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9f9b7-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9f9b7-119">Schema name</span></span>  <br/> |<span data-ttu-id="9f9b7-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="9f9b7-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9f9b7-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9f9b7-121">Validation file</span></span>  <br/> |<span data-ttu-id="9f9b7-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9f9b7-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9f9b7-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="9f9b7-123">Can be empty</span></span>  <br/> |<span data-ttu-id="9f9b7-124">falso</span><span class="sxs-lookup"><span data-stu-id="9f9b7-124">false</span></span>  <br/> |
   

