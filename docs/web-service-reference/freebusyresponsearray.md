---
title: FreeBusyResponseArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyResponseArray
api_type:
- schema
ms.assetid: 5592a37e-cf4b-4643-8a2a-fa58c40345b9
description: O elemento FreeBusyResponseArray contém as informações de disponibilidade dos usuários solicitados e o status da resposta.
ms.openlocfilehash: b45938c19b76a377fca125fb6a19f9d712718db6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457806"
---
# <a name="freebusyresponsearray"></a><span data-ttu-id="4551f-103">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="4551f-103">FreeBusyResponseArray</span></span>

<span data-ttu-id="4551f-104">O elemento **FreeBusyResponseArray** contém as informações de disponibilidade dos usuários solicitados e o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="4551f-104">The **FreeBusyResponseArray** element contains the requested users' availability information and the response status.</span></span> 
  
[<span data-ttu-id="4551f-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="4551f-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="4551f-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="4551f-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
```xml
<FreeBusyResponseArray>
   <FreeBusyResponse>...</FreeBusyResponse>
</FreeBusyResponseArray>
```

 <span data-ttu-id="4551f-107">**ArrayOfFreeBusyResponse**</span><span class="sxs-lookup"><span data-stu-id="4551f-107">**ArrayOfFreeBusyResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4551f-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4551f-108">Attributes and elements</span></span>

<span data-ttu-id="4551f-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4551f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4551f-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="4551f-110">Attributes</span></span>

<span data-ttu-id="4551f-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4551f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4551f-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4551f-112">Child elements</span></span>

|<span data-ttu-id="4551f-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4551f-113">**Element**</span></span>|<span data-ttu-id="4551f-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4551f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4551f-115">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="4551f-115">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="4551f-116">Contém as informações de disponibilidade de um único usuário de caixa de correio e o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="4551f-116">Contains the free/busy information for a single mailbox user and the response status.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4551f-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4551f-117">Parent elements</span></span>

|<span data-ttu-id="4551f-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4551f-118">**Element**</span></span>|<span data-ttu-id="4551f-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4551f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4551f-120">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="4551f-120">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) <br/> |<span data-ttu-id="4551f-121">Contém as propriedades que definem informações de disponibilidade do usuário ou informações de tempo de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="4551f-121">Contains the properties that define user availability information or suggested meeting time information.</span></span>  <br/> <span data-ttu-id="4551f-122">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="4551f-122">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4551f-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="4551f-123">Remarks</span></span>

<span data-ttu-id="4551f-124">Esse elemento não está incluído em uma resposta GetUserAvailability se não for solicitada informação de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="4551f-124">This element is not included in a GetUserAvailability response if free/busy information is not requested.</span></span>
  
<span data-ttu-id="4551f-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="4551f-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4551f-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4551f-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4551f-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="4551f-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4551f-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4551f-128">Schema Name</span></span>  <br/> |<span data-ttu-id="4551f-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="4551f-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4551f-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4551f-130">Validation File</span></span>  <br/> |<span data-ttu-id="4551f-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4551f-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4551f-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4551f-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="4551f-133">False</span><span class="sxs-lookup"><span data-stu-id="4551f-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4551f-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="4551f-134">See also</span></span>



[<span data-ttu-id="4551f-135">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="4551f-135">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="4551f-136">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="4551f-136">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="4551f-137">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="4551f-137">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

