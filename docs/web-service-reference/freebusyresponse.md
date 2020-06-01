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
description: O elemento FreeBusyResponse contém as informações de disponibilidade de um único usuário de caixa de correio.
ms.openlocfilehash: 45a3e12756f3cbf29b76b442f7103abc5fb9a833
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461923"
---
# <a name="freebusyresponse"></a><span data-ttu-id="634a8-103">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="634a8-103">FreeBusyResponse</span></span>

<span data-ttu-id="634a8-104">O elemento **FreeBusyResponse** contém as informações de disponibilidade de um único usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="634a8-104">The **FreeBusyResponse** element contains the free/busy information for a single mailbox user.</span></span> 
  
[<span data-ttu-id="634a8-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="634a8-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="634a8-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="634a8-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="634a8-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="634a8-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
```xml
<FreeBusyResponse>
   <ResponseMessage>...</ResponseMessage>
   <FreeBusyView>...</FreeBusyView>
</FreeBusyResponse>
```

 <span data-ttu-id="634a8-108">**FreeBusyResponseType**</span><span class="sxs-lookup"><span data-stu-id="634a8-108">**FreeBusyResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="634a8-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="634a8-109">Attributes and elements</span></span>

<span data-ttu-id="634a8-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="634a8-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="634a8-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="634a8-111">Attributes</span></span>

<span data-ttu-id="634a8-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="634a8-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="634a8-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="634a8-113">Child elements</span></span>

|<span data-ttu-id="634a8-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="634a8-114">**Element**</span></span>|<span data-ttu-id="634a8-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="634a8-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="634a8-116">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="634a8-116">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="634a8-117">Fornece informações descritivas sobre o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="634a8-117">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="634a8-118">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="634a8-118">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="634a8-119">Contém informações de disponibilidade para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="634a8-119">Contains availability information for a specific user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="634a8-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="634a8-120">Parent elements</span></span>

|<span data-ttu-id="634a8-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="634a8-121">**Element**</span></span>|<span data-ttu-id="634a8-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="634a8-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="634a8-123">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="634a8-123">FreeBusyResponseArray</span></span>](freebusyresponsearray.md) <br/> |<span data-ttu-id="634a8-124">Contém as informações de disponibilidade dos usuários solicitados e o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="634a8-124">Contains the requested users' availability information and the response status.</span></span>  <br/> <span data-ttu-id="634a8-125">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="634a8-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="634a8-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="634a8-126">Remarks</span></span>

<span data-ttu-id="634a8-127">Esse elemento não está incluído em uma resposta GetUserAvailability se não for solicitada informação de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="634a8-127">This element is not included in a GetUserAvailability response if free/busy information is not requested.</span></span>
  
<span data-ttu-id="634a8-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="634a8-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="634a8-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="634a8-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="634a8-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="634a8-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="634a8-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="634a8-131">Schema Name</span></span>  <br/> |<span data-ttu-id="634a8-132">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="634a8-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="634a8-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="634a8-133">Validation File</span></span>  <br/> |<span data-ttu-id="634a8-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="634a8-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="634a8-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="634a8-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="634a8-136">False</span><span class="sxs-lookup"><span data-stu-id="634a8-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="634a8-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="634a8-137">See also</span></span>



[<span data-ttu-id="634a8-138">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="634a8-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="634a8-139">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="634a8-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="634a8-140">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="634a8-140">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

