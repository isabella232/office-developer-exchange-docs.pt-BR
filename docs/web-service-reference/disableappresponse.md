---
title: DisableAppResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 11ebe618-d759-4f16-be99-eaaa817ba782
description: O elemento DisableAppResponse especifica a resposta a uma solicitação DisableApp.
ms.openlocfilehash: cc28abf644247339e1226cd0e13824cc5f5669be
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455643"
---
# <a name="disableappresponse"></a><span data-ttu-id="4d268-103">DisableAppResponse</span><span class="sxs-lookup"><span data-stu-id="4d268-103">DisableAppResponse</span></span>

<span data-ttu-id="4d268-104">O elemento **DisableAppResponse** especifica a resposta a uma solicitação **DisableApp** .</span><span class="sxs-lookup"><span data-stu-id="4d268-104">The **DisableAppResponse** element specifies the response to a **DisableApp** request.</span></span> 
  
```XML
<DisableAppResponse>
    <MessageText></MessageText>
    <ResponseCode></ResponeCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</DisableAppResponse>
```

 <span data-ttu-id="4d268-105">**DisableAppResponseType**</span><span class="sxs-lookup"><span data-stu-id="4d268-105">**DisableAppResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4d268-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4d268-106">Attributes and elements</span></span>

<span data-ttu-id="4d268-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4d268-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d268-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4d268-108">Attributes</span></span>

<span data-ttu-id="4d268-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4d268-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4d268-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4d268-110">Child elements</span></span>

|<span data-ttu-id="4d268-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4d268-111">**Element**</span></span>|<span data-ttu-id="4d268-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4d268-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d268-113">MessageText</span><span class="sxs-lookup"><span data-stu-id="4d268-113">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="4d268-114">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d268-114">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="4d268-115">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4d268-115">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="4d268-116">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d268-116">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="4d268-117">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="4d268-117">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="4d268-118">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="4d268-118">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="4d268-119">MessageXml</span><span class="sxs-lookup"><span data-stu-id="4d268-119">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="4d268-120">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="4d268-120">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4d268-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4d268-121">Parent elements</span></span>

<span data-ttu-id="4d268-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4d268-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4d268-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="4d268-123">Remarks</span></span>

<span data-ttu-id="4d268-124">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4d268-124">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4d268-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d268-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d268-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4d268-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d268-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="4d268-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4d268-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4d268-128">Schema Name</span></span>  <br/> |<span data-ttu-id="4d268-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="4d268-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="4d268-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4d268-130">Validation File</span></span>  <br/> |<span data-ttu-id="4d268-131">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4d268-131">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4d268-132">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="4d268-132">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4d268-133">Também consulte</span><span class="sxs-lookup"><span data-stu-id="4d268-133">See also</span></span>

- [<span data-ttu-id="4d268-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4d268-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

