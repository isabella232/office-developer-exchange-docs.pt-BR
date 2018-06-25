---
title: GetDelegateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetDelegateResponse
api_type:
- schema
ms.assetid: 71a418a5-5652-40e1-8f84-fe4f7c9f86af
description: O elemento GetDelegateResponse contém o status e o resultado de uma solicitação de operação GetDelegate.
ms.openlocfilehash: 52731ea66420c21cf3fb8d19082aef65551c2af2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752454"
---
# <a name="getdelegateresponse"></a><span data-ttu-id="c247a-103">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="c247a-103">GetDelegateResponse</span></span>

<span data-ttu-id="c247a-104">O elemento **GetDelegateResponse** contém o status e o resultado de uma solicitação de [operação GetDelegate](getdelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="c247a-104">The **GetDelegateResponse** element contains the status and result of a [GetDelegate operation](getdelegate-operation.md) request.</span></span> 
  
```xml
<GetDelegateResponse>
   <DeliverMeetingRequests/>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</GetDelegateResponse>
```

 <span data-ttu-id="c247a-105">**GetDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="c247a-105">**GetDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c247a-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c247a-106">Attributes and elements</span></span>

<span data-ttu-id="c247a-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c247a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c247a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c247a-108">Attributes</span></span>

<span data-ttu-id="c247a-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c247a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c247a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c247a-110">Child elements</span></span>

|<span data-ttu-id="c247a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c247a-111">**Element**</span></span>|<span data-ttu-id="c247a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c247a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c247a-113">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="c247a-113">DeliverMeetingRequests</span></span>](delivermeetingrequests.md) <br/> |<span data-ttu-id="c247a-114">Define como as solicitações de reunião são manipuladas entre o delegado e a entidade.</span><span class="sxs-lookup"><span data-stu-id="c247a-114">Defines how meeting requests are handled between the delegate and the principal.</span></span>  <br/> |
|[<span data-ttu-id="c247a-115">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="c247a-115">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="c247a-116">Contém as mensagens de resposta para uma solicitação de gerenciamento do representante de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c247a-116">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="c247a-117">MessageText</span><span class="sxs-lookup"><span data-stu-id="c247a-117">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="c247a-118">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="c247a-118">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="c247a-119">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c247a-119">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="c247a-120">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="c247a-120">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="c247a-121">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c247a-121">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="c247a-122">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="c247a-122">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="c247a-123">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="c247a-123">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="c247a-124">MessageXml</span><span class="sxs-lookup"><span data-stu-id="c247a-124">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="c247a-125">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="c247a-125">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c247a-126">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c247a-126">Parent elements</span></span>

<span data-ttu-id="c247a-127">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c247a-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c247a-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="c247a-128">Remarks</span></span>

<span data-ttu-id="c247a-129">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="c247a-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c247a-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c247a-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c247a-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="c247a-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c247a-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c247a-132">Schema Name</span></span>  <br/> |<span data-ttu-id="c247a-133">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c247a-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c247a-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c247a-134">Validation File</span></span>  <br/> |<span data-ttu-id="c247a-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c247a-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c247a-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c247a-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="c247a-137">False</span><span class="sxs-lookup"><span data-stu-id="c247a-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c247a-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="c247a-138">See also</span></span>



[<span data-ttu-id="c247a-139">Operação GetDelegate</span><span class="sxs-lookup"><span data-stu-id="c247a-139">GetDelegate operation</span></span>](getdelegate-operation.md)


- [<span data-ttu-id="c247a-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c247a-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

