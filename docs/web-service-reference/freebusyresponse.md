---
title: FreeBusyResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyResponse
api_type:
- schema
ms.assetid: 3038d106-9ac9-4ac7-bb43-96c783edbef5
description: O elemento FreeBusyResponse contém as informações de disponibilidade para um usuário de caixa de correio única.
ms.openlocfilehash: 73e3972bb53d6bf59e5156098bad06bcde5f0155
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752365"
---
# <a name="freebusyresponse"></a><span data-ttu-id="76166-103">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="76166-103">FreeBusyResponse</span></span>

<span data-ttu-id="76166-104">O elemento **FreeBusyResponse** contém as informações de disponibilidade para um usuário de caixa de correio única.</span><span class="sxs-lookup"><span data-stu-id="76166-104">The **FreeBusyResponse** element contains the free/busy information for a single mailbox user.</span></span> 
  
[<span data-ttu-id="76166-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="76166-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="76166-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="76166-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="76166-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="76166-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
```xml
<FreeBusyResponse>
   <ResponseMessage>...</ResponseMessage>
   <FreeBusyView>...</FreeBusyView>
</FreeBusyResponse>
```

 <span data-ttu-id="76166-108">**FreeBusyResponseType**</span><span class="sxs-lookup"><span data-stu-id="76166-108">**FreeBusyResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="76166-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="76166-109">Attributes and elements</span></span>

<span data-ttu-id="76166-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="76166-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76166-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="76166-111">Attributes</span></span>

<span data-ttu-id="76166-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="76166-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="76166-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="76166-113">Child elements</span></span>

|<span data-ttu-id="76166-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="76166-114">**Element**</span></span>|<span data-ttu-id="76166-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="76166-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76166-116">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76166-116">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="76166-117">Fornece informações descritivas sobre o status de resposta.</span><span class="sxs-lookup"><span data-stu-id="76166-117">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="76166-118">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="76166-118">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="76166-119">Contém informações de disponibilidade para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="76166-119">Contains availability information for a specific user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="76166-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="76166-120">Parent elements</span></span>

|<span data-ttu-id="76166-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="76166-121">**Element**</span></span>|<span data-ttu-id="76166-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="76166-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76166-123">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="76166-123">FreeBusyResponseArray</span></span>](freebusyresponsearray.md) <br/> |<span data-ttu-id="76166-124">Contém informações de disponibilidade dos usuários solicitado e o status de resposta.</span><span class="sxs-lookup"><span data-stu-id="76166-124">Contains the requested users' availability information and the response status.</span></span>  <br/> <span data-ttu-id="76166-125">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="76166-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="76166-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="76166-126">Remarks</span></span>

<span data-ttu-id="76166-127">Esse elemento não está incluído em uma resposta GetUserAvailability se as informações de disponibilidade não são solicitadas.</span><span class="sxs-lookup"><span data-stu-id="76166-127">This element is not included in a GetUserAvailability response if free/busy information is not requested.</span></span>
  
<span data-ttu-id="76166-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="76166-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76166-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="76166-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76166-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="76166-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="76166-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="76166-131">Schema Name</span></span>  <br/> |<span data-ttu-id="76166-132">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="76166-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="76166-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="76166-133">Validation File</span></span>  <br/> |<span data-ttu-id="76166-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="76166-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="76166-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="76166-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="76166-136">False</span><span class="sxs-lookup"><span data-stu-id="76166-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="76166-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="76166-137">See also</span></span>



[<span data-ttu-id="76166-138">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="76166-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="76166-139">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="76166-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="76166-140">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="76166-140">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

