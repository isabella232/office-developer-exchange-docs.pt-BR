---
title: SetHoldOnMailboxesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d61de0f3-24e0-434a-946a-c53d393b7d04
description: O elemento SetHoldOnMailboxesResponseMessage Especifica a mensagem de resposta para uma solicitação de SetHoldOnMailboxes.
ms.openlocfilehash: b7cb890a71d27340e328e39c1c463fefa080b8cb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825420"
---
# <a name="setholdonmailboxesresponsemessage"></a><span data-ttu-id="922b1-103">SetHoldOnMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="922b1-103">SetHoldOnMailboxesResponseMessage</span></span>

<span data-ttu-id="922b1-104">O elemento **SetHoldOnMailboxesResponseMessage** Especifica a mensagem de resposta para uma solicitação de **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="922b1-104">The **SetHoldOnMailboxesResponseMessage** element specifies the response message for a **SetHoldOnMailboxes** request.</span></span> 
  
```XML
<SetHoldOnMailboxesResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailboxHoldResult/>
</SetHoldOnMailboxesResponseMessage>
```

 <span data-ttu-id="922b1-105">**SetHoldOnMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="922b1-105">**SetHoldOnMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="922b1-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="922b1-106">Attributes and elements</span></span>

<span data-ttu-id="922b1-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="922b1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="922b1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="922b1-108">Attributes</span></span>

<span data-ttu-id="922b1-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="922b1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="922b1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="922b1-110">Child elements</span></span>

<span data-ttu-id="922b1-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MailboxHoldResult](mailboxholdresult.md)</span><span class="sxs-lookup"><span data-stu-id="922b1-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MailboxHoldResult](mailboxholdresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="922b1-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="922b1-112">Parent elements</span></span>

[<span data-ttu-id="922b1-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="922b1-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="922b1-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="922b1-114">Remarks</span></span>

<span data-ttu-id="922b1-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="922b1-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="922b1-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="922b1-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="922b1-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="922b1-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="922b1-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="922b1-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="922b1-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="922b1-119">Schema name</span></span>  <br/> |<span data-ttu-id="922b1-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="922b1-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="922b1-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="922b1-121">Validation file</span></span>  <br/> |<span data-ttu-id="922b1-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="922b1-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="922b1-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="922b1-123">Can be empty</span></span>  <br/> ||
   

