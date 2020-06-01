---
title: GetPersonaResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a5bf44c6-c46b-442d-98d4-8b49fdf14b30
description: O GetPersonaResponseMessage contém os dados de resposta resultantes de uma solicitação getpersona.
ms.openlocfilehash: 6391e1b6682180e292d03c5db651e8edc6f46b52
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458324"
---
# <a name="getpersonaresponsemessage"></a><span data-ttu-id="190ba-103">GetPersonaResponseMessage</span><span class="sxs-lookup"><span data-stu-id="190ba-103">GetPersonaResponseMessage</span></span>

<span data-ttu-id="190ba-104">O **GetPersonaResponseMessage** contém os dados de resposta resultantes de uma solicitação **getpersona** .</span><span class="sxs-lookup"><span data-stu-id="190ba-104">The **GetPersonaResponseMessage** contains the response data resulting from a **GetPersona** request.</span></span> 
  
```XML
<GetPersonaResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Persona/>
</GetPersonaResponseMessage>
```

 <span data-ttu-id="190ba-105">**GetUserPhotoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="190ba-105">**GetUserPhotoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="190ba-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="190ba-106">Attributes and elements</span></span>

<span data-ttu-id="190ba-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="190ba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="190ba-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="190ba-108">Attributes</span></span>

<span data-ttu-id="190ba-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="190ba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="190ba-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="190ba-110">Child elements</span></span>

<span data-ttu-id="190ba-111">[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [DescriptiveLinkKey](descriptivelinkkey.md)  |  [MessageXml](messagexml.md)  |  [Persona](persona.md)</span><span class="sxs-lookup"><span data-stu-id="190ba-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [Persona](persona.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="190ba-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="190ba-112">Parent elements</span></span>

[<span data-ttu-id="190ba-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="190ba-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="190ba-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="190ba-114">Remarks</span></span>

<span data-ttu-id="190ba-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="190ba-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="190ba-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="190ba-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="190ba-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="190ba-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="190ba-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="190ba-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="190ba-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="190ba-119">Schema name</span></span>  <br/> |<span data-ttu-id="190ba-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="190ba-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="190ba-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="190ba-121">Validation file</span></span>  <br/> |<span data-ttu-id="190ba-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="190ba-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="190ba-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="190ba-123">Can be empty</span></span>  <br/> ||
   

