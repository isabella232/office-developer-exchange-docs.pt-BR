---
title: RemoveDelegateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveDelegateResponse
api_type:
- schema
ms.assetid: eef56c53-d0a7-4342-9ce6-4dbb6b1a1369
description: O elemento RemoveDelegateResponse contém o status e o resultado de uma solicitação de operação RemoveDelegate.
ms.openlocfilehash: 45d0bcfaeb4d453f50cce8449f5cb7fdb70512a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825092"
---
# <a name="removedelegateresponse"></a><span data-ttu-id="1273b-103">RemoveDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="1273b-103">RemoveDelegateResponse</span></span>

<span data-ttu-id="1273b-104">O elemento **RemoveDelegateResponse** contém o status e o resultado de uma solicitação de [operação RemoveDelegate](removedelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1273b-104">The **RemoveDelegateResponse** element contains the status and result of a [RemoveDelegate operation](removedelegate-operation.md) request.</span></span> 
  
```xml
<RemoveDelegateResponse>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RemoveDelegateResponse>
```

 <span data-ttu-id="1273b-105">**RemoveDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1273b-105">**RemoveDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1273b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1273b-106">Attributes and elements</span></span>

<span data-ttu-id="1273b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1273b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1273b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1273b-108">Attributes</span></span>

<span data-ttu-id="1273b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1273b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1273b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1273b-110">Child elements</span></span>

|<span data-ttu-id="1273b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1273b-111">**Element**</span></span>|<span data-ttu-id="1273b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1273b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1273b-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="1273b-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="1273b-114">Contém as mensagens de resposta para uma solicitação de gerenciamento do representante de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1273b-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="1273b-115">MessageText</span><span class="sxs-lookup"><span data-stu-id="1273b-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="1273b-116">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="1273b-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="1273b-117">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1273b-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="1273b-118">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="1273b-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="1273b-119">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1273b-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="1273b-120">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="1273b-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="1273b-121">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="1273b-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="1273b-122">MessageXml</span><span class="sxs-lookup"><span data-stu-id="1273b-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="1273b-123">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="1273b-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1273b-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1273b-124">Parent elements</span></span>

<span data-ttu-id="1273b-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1273b-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1273b-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="1273b-126">Remarks</span></span>

<span data-ttu-id="1273b-127">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="1273b-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1273b-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="1273b-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1273b-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="1273b-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1273b-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1273b-130">Schema Name</span></span>  <br/> |<span data-ttu-id="1273b-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="1273b-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1273b-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1273b-132">Validation File</span></span>  <br/> |<span data-ttu-id="1273b-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1273b-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1273b-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1273b-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="1273b-135">False</span><span class="sxs-lookup"><span data-stu-id="1273b-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1273b-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="1273b-136">See also</span></span>



[<span data-ttu-id="1273b-137">Operação RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="1273b-137">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="1273b-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1273b-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

