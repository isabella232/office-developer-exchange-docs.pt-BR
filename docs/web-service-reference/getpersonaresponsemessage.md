---
title: GetPersonaResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a5bf44c6-c46b-442d-98d4-8b49fdf14b30
description: O GetPersonaResponseMessage contém os dados de resposta resultante de uma solicitação de GetPersona.
ms.openlocfilehash: 7d38daac9c7c3a74ba9d9670c2bd16dcf2cd47e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752601"
---
# <a name="getpersonaresponsemessage"></a><span data-ttu-id="30b10-103">GetPersonaResponseMessage</span><span class="sxs-lookup"><span data-stu-id="30b10-103">GetPersonaResponseMessage</span></span>

<span data-ttu-id="30b10-104">O **GetPersonaResponseMessage** contém os dados de resposta resultante de uma solicitação de **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="30b10-104">The **GetPersonaResponseMessage** contains the response data resulting from a **GetPersona** request.</span></span> 
  
```XML
<GetPersonaResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Persona/>
</GetPersonaResponseMessage>
```

 <span data-ttu-id="30b10-105">**GetUserPhotoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="30b10-105">**GetUserPhotoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="30b10-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="30b10-106">Attributes and elements</span></span>

<span data-ttu-id="30b10-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="30b10-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30b10-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="30b10-108">Attributes</span></span>

<span data-ttu-id="30b10-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="30b10-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="30b10-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="30b10-110">Child elements</span></span>

<span data-ttu-id="30b10-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [pessoa](persona.md)</span><span class="sxs-lookup"><span data-stu-id="30b10-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [Persona](persona.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="30b10-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="30b10-112">Parent elements</span></span>

[<span data-ttu-id="30b10-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="30b10-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="30b10-114">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="30b10-114">Remarks</span></span>

<span data-ttu-id="30b10-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="30b10-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="30b10-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="30b10-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30b10-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="30b10-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30b10-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="30b10-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="30b10-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="30b10-119">Schema name</span></span>  <br/> |<span data-ttu-id="30b10-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="30b10-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="30b10-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="30b10-121">Validation file</span></span>  <br/> |<span data-ttu-id="30b10-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="30b10-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="30b10-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="30b10-123">Can be empty</span></span>  <br/> ||
   

