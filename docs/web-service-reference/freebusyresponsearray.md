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
description: O elemento FreeBusyResponseArray contém informações de disponibilidade dos usuários solicitado e o status de resposta.
ms.openlocfilehash: cc6022c28213667c40dc00b5627ed88c4f78e2f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752368"
---
# <a name="freebusyresponsearray"></a><span data-ttu-id="123f5-103">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="123f5-103">FreeBusyResponseArray</span></span>

<span data-ttu-id="123f5-104">O elemento **FreeBusyResponseArray** contém informações de disponibilidade dos usuários solicitado e o status de resposta.</span><span class="sxs-lookup"><span data-stu-id="123f5-104">The **FreeBusyResponseArray** element contains the requested users' availability information and the response status.</span></span> 
  
[<span data-ttu-id="123f5-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="123f5-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="123f5-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="123f5-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
```xml
<FreeBusyResponseArray>
   <FreeBusyResponse>...</FreeBusyResponse>
</FreeBusyResponseArray>
```

 <span data-ttu-id="123f5-107">**ArrayOfFreeBusyResponse**</span><span class="sxs-lookup"><span data-stu-id="123f5-107">**ArrayOfFreeBusyResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="123f5-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="123f5-108">Attributes and elements</span></span>

<span data-ttu-id="123f5-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="123f5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="123f5-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="123f5-110">Attributes</span></span>

<span data-ttu-id="123f5-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="123f5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="123f5-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="123f5-112">Child elements</span></span>

|<span data-ttu-id="123f5-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="123f5-113">**Element**</span></span>|<span data-ttu-id="123f5-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="123f5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="123f5-115">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="123f5-115">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="123f5-116">Contém as informações de disponibilidade para um usuário de caixa de correio única e o status de resposta.</span><span class="sxs-lookup"><span data-stu-id="123f5-116">Contains the free/busy information for a single mailbox user and the response status.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="123f5-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="123f5-117">Parent elements</span></span>

|<span data-ttu-id="123f5-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="123f5-118">**Element**</span></span>|<span data-ttu-id="123f5-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="123f5-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="123f5-120">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="123f5-120">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) <br/> |<span data-ttu-id="123f5-121">Contém as propriedades que definem as informações de disponibilidade do usuário ou sugerido informações de tempo da reunião.</span><span class="sxs-lookup"><span data-stu-id="123f5-121">Contains the properties that define user availability information or suggested meeting time information.</span></span>  <br/> <span data-ttu-id="123f5-122">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="123f5-122">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="123f5-123">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="123f5-123">Remarks</span></span>

<span data-ttu-id="123f5-124">Esse elemento não está incluído em uma resposta GetUserAvailability se as informações de disponibilidade não são solicitadas.</span><span class="sxs-lookup"><span data-stu-id="123f5-124">This element is not included in a GetUserAvailability response if free/busy information is not requested.</span></span>
  
<span data-ttu-id="123f5-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="123f5-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="123f5-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="123f5-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="123f5-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="123f5-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="123f5-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="123f5-128">Schema Name</span></span>  <br/> |<span data-ttu-id="123f5-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="123f5-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="123f5-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="123f5-130">Validation File</span></span>  <br/> |<span data-ttu-id="123f5-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="123f5-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="123f5-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="123f5-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="123f5-133">False</span><span class="sxs-lookup"><span data-stu-id="123f5-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="123f5-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="123f5-134">See also</span></span>



[<span data-ttu-id="123f5-135">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="123f5-135">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="123f5-136">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="123f5-136">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="123f5-137">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="123f5-137">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

