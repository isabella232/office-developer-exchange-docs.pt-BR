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
ms.openlocfilehash: 4c7a8b81528435b72576c116bc97f611544c24d6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468933"
---
# <a name="removedelegateresponse"></a><span data-ttu-id="383ca-103">RemoveDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="383ca-103">RemoveDelegateResponse</span></span>

<span data-ttu-id="383ca-104">O elemento **RemoveDelegateResponse** contém o status e o resultado de uma solicitação de [operação RemoveDelegate](removedelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="383ca-104">The **RemoveDelegateResponse** element contains the status and result of a [RemoveDelegate operation](removedelegate-operation.md) request.</span></span> 
  
```xml
<RemoveDelegateResponse>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RemoveDelegateResponse>
```

 <span data-ttu-id="383ca-105">**RemoveDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="383ca-105">**RemoveDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="383ca-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="383ca-106">Attributes and elements</span></span>

<span data-ttu-id="383ca-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="383ca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="383ca-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="383ca-108">Attributes</span></span>

<span data-ttu-id="383ca-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="383ca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="383ca-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="383ca-110">Child elements</span></span>

|<span data-ttu-id="383ca-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="383ca-111">**Element**</span></span>|<span data-ttu-id="383ca-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="383ca-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="383ca-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="383ca-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="383ca-114">Contém as mensagens de resposta para uma solicitação de gerenciamento de representante do Exchange Web Services.</span><span class="sxs-lookup"><span data-stu-id="383ca-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="383ca-115">MessageText</span><span class="sxs-lookup"><span data-stu-id="383ca-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="383ca-116">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="383ca-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="383ca-117">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="383ca-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="383ca-118">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="383ca-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="383ca-119">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="383ca-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="383ca-120">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="383ca-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="383ca-121">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="383ca-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="383ca-122">MessageXml</span><span class="sxs-lookup"><span data-stu-id="383ca-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="383ca-123">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="383ca-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="383ca-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="383ca-124">Parent elements</span></span>

<span data-ttu-id="383ca-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="383ca-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="383ca-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="383ca-126">Remarks</span></span>

<span data-ttu-id="383ca-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="383ca-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="383ca-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="383ca-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="383ca-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="383ca-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="383ca-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="383ca-130">Schema Name</span></span>  <br/> |<span data-ttu-id="383ca-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="383ca-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="383ca-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="383ca-132">Validation File</span></span>  <br/> |<span data-ttu-id="383ca-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="383ca-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="383ca-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="383ca-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="383ca-135">False</span><span class="sxs-lookup"><span data-stu-id="383ca-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="383ca-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="383ca-136">See also</span></span>



[<span data-ttu-id="383ca-137">Operação RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="383ca-137">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="383ca-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="383ca-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

