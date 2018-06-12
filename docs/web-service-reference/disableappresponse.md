---
title: DisableAppResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 11ebe618-d759-4f16-be99-eaaa817ba782
description: O elemento DisableAppResponse Especifica a resposta a uma solicitação DisableApp.
ms.openlocfilehash: 740801fa4b60e217f0b9148bcfcc5b206e96bf31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751833"
---
# <a name="disableappresponse"></a><span data-ttu-id="28423-103">DisableAppResponse</span><span class="sxs-lookup"><span data-stu-id="28423-103">DisableAppResponse</span></span>

<span data-ttu-id="28423-104">O elemento **DisableAppResponse** Especifica a resposta a uma solicitação **DisableApp** .</span><span class="sxs-lookup"><span data-stu-id="28423-104">The **DisableAppResponse** element specifies the response to a **DisableApp** request.</span></span> 
  
```XML
<DisableAppResponse>
    <MessageText></MessageText>
    <ResponseCode></ResponeCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</DisableAppResponse>
```

 <span data-ttu-id="28423-105">**DisableAppResponseType**</span><span class="sxs-lookup"><span data-stu-id="28423-105">**DisableAppResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28423-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="28423-106">Attributes and elements</span></span>

<span data-ttu-id="28423-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="28423-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28423-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="28423-108">Attributes</span></span>

<span data-ttu-id="28423-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="28423-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="28423-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="28423-110">Child elements</span></span>

|<span data-ttu-id="28423-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="28423-111">**Element**</span></span>|<span data-ttu-id="28423-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="28423-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28423-113">MessageText</span><span class="sxs-lookup"><span data-stu-id="28423-113">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="28423-114">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="28423-114">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="28423-115">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="28423-115">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="28423-116">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="28423-116">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="28423-117">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="28423-117">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="28423-118">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="28423-118">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="28423-119">MessageXml</span><span class="sxs-lookup"><span data-stu-id="28423-119">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="28423-120">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="28423-120">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="28423-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="28423-121">Parent elements</span></span>

<span data-ttu-id="28423-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="28423-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="28423-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="28423-123">Remarks</span></span>

<span data-ttu-id="28423-124">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="28423-124">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="28423-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="28423-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28423-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="28423-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28423-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="28423-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="28423-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="28423-128">Schema Name</span></span>  <br/> |<span data-ttu-id="28423-129">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="28423-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="28423-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="28423-130">Validation File</span></span>  <br/> |<span data-ttu-id="28423-131">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="28423-131">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="28423-132">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="28423-132">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="28423-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="28423-133">See also</span></span>

- [<span data-ttu-id="28423-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="28423-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

