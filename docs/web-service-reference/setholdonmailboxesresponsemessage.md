---
title: SetHoldOnMailboxesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d61de0f3-24e0-434a-946a-c53d393b7d04
description: O elemento SetHoldOnMailboxesResponseMessage especifica a mensagem de resposta para uma solicitação SetHoldOnMailboxes.
ms.openlocfilehash: a6af4181218391bc9d3c177467295d771cce4c89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456406"
---
# <a name="setholdonmailboxesresponsemessage"></a><span data-ttu-id="d3b55-103">SetHoldOnMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d3b55-103">SetHoldOnMailboxesResponseMessage</span></span>

<span data-ttu-id="d3b55-104">O elemento **SetHoldOnMailboxesResponseMessage** especifica a mensagem de resposta para uma solicitação **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="d3b55-104">The **SetHoldOnMailboxesResponseMessage** element specifies the response message for a **SetHoldOnMailboxes** request.</span></span> 
  
```XML
<SetHoldOnMailboxesResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailboxHoldResult/>
</SetHoldOnMailboxesResponseMessage>
```

 <span data-ttu-id="d3b55-105">**SetHoldOnMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d3b55-105">**SetHoldOnMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3b55-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d3b55-106">Attributes and elements</span></span>

<span data-ttu-id="d3b55-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d3b55-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3b55-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d3b55-108">Attributes</span></span>

<span data-ttu-id="d3b55-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d3b55-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3b55-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d3b55-110">Child elements</span></span>

<span data-ttu-id="d3b55-111">[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [DescriptiveLinkKey](descriptivelinkkey.md)  |  [MessageXml](messagexml.md)  |  [MailboxHoldResult](mailboxholdresult.md)</span><span class="sxs-lookup"><span data-stu-id="d3b55-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MailboxHoldResult](mailboxholdresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d3b55-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d3b55-112">Parent elements</span></span>

[<span data-ttu-id="d3b55-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d3b55-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="d3b55-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="d3b55-114">Remarks</span></span>

<span data-ttu-id="d3b55-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d3b55-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d3b55-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3b55-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3b55-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d3b55-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3b55-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="d3b55-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d3b55-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d3b55-119">Schema name</span></span>  <br/> |<span data-ttu-id="d3b55-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d3b55-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d3b55-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d3b55-121">Validation file</span></span>  <br/> |<span data-ttu-id="d3b55-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d3b55-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d3b55-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d3b55-123">Can be empty</span></span>  <br/> ||
   

