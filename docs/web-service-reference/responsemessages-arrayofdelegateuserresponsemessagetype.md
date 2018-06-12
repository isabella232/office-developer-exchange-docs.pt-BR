---
title: ResponseMessages (ArrayOfDelegateUserResponseMessageType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 14819975-ce54-4f0e-9f90-d4b275895ea0
description: O elemento ResponseMessages contém as mensagens de resposta para uma solicitação de gerenciamento do representante de serviços Web do Exchange.
ms.openlocfilehash: e4b5567f3ded003e9648eb8ebebfadf8f1748d6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825193"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a><span data-ttu-id="55d0c-103">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="55d0c-103">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>

<span data-ttu-id="55d0c-104">O elemento **ResponseMessages** contém as mensagens de resposta para uma solicitação de gerenciamento do representante de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="55d0c-104">The **ResponseMessages** element contains the response messages for an Exchange Web Services delegate management request.</span></span> 
  
```
<ResponseMessages>
   <DelegateUserResponseMessageType/>
</ResponseMessages>
```

 <span data-ttu-id="55d0c-105">**ArrayOfDelegateUserResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="55d0c-105">**ArrayOfDelegateUserResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55d0c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="55d0c-106">Attributes and elements</span></span>

<span data-ttu-id="55d0c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="55d0c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55d0c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="55d0c-108">Attributes</span></span>

<span data-ttu-id="55d0c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="55d0c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55d0c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="55d0c-110">Child elements</span></span>

|<span data-ttu-id="55d0c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="55d0c-111">**Element**</span></span>|<span data-ttu-id="55d0c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="55d0c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55d0c-113">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="55d0c-113">DelegateUserResponseMessageType</span></span>](delegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="55d0c-114">Contém mensagens de resposta para operações de gerenciamento de representante.</span><span class="sxs-lookup"><span data-stu-id="55d0c-114">Contains response messages for delegate management operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="55d0c-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="55d0c-115">Parent elements</span></span>

|<span data-ttu-id="55d0c-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="55d0c-116">**Element**</span></span>|<span data-ttu-id="55d0c-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="55d0c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55d0c-118">AddDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="55d0c-118">AddDelegateResponse</span></span>](adddelegateresponse.md) <br/> |<span data-ttu-id="55d0c-119">Contém o status e o resultado de uma solicitação de [operação AddDelegate](adddelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="55d0c-119">Contains the status and result of an [AddDelegate operation](adddelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="55d0c-120">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="55d0c-120">GetDelegateResponse</span></span>](getdelegateresponse.md) <br/> |<span data-ttu-id="55d0c-121">Contém o status e o resultado de uma solicitação de [operação GetDelegate](getdelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="55d0c-121">Contains the status and result of a [GetDelegate operation](getdelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="55d0c-122">UpdateDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="55d0c-122">UpdateDelegateResponse</span></span>](updatedelegateresponse.md) <br/> |<span data-ttu-id="55d0c-123">Contém o status e o resultado de uma solicitação de [operação UpdateDelegate](updatedelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="55d0c-123">Contains the status and result of an [UpdateDelegate operation](updatedelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="55d0c-124">RemoveDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="55d0c-124">RemoveDelegateResponse</span></span>](removedelegateresponse.md) <br/> |<span data-ttu-id="55d0c-125">Contém o status e o resultado de uma solicitação de [operação RemoveDelegate](removedelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="55d0c-125">Contains the status and result of a [RemoveDelegate operation](removedelegate-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="55d0c-126">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="55d0c-126">Remarks</span></span>

<span data-ttu-id="55d0c-127">Esse elemento é usado a [operação AddDelegate](adddelegate-operation.md), a [operação de GetDelegate](getdelegate-operation.md), a [operação UpdateDelegate](updatedelegate-operation.md)e a [operação RemoveDelegate](removedelegate-operation.md).</span><span class="sxs-lookup"><span data-stu-id="55d0c-127">This element is used in the [AddDelegate operation](adddelegate-operation.md), the [GetDelegate operation](getdelegate-operation.md), the [UpdateDelegate operation](updatedelegate-operation.md), and the [RemoveDelegate operation](removedelegate-operation.md).</span></span> <span data-ttu-id="55d0c-128">As respostas de operação de gerenciamento de representante são estruturadas de forma diferente de outras respostas.</span><span class="sxs-lookup"><span data-stu-id="55d0c-128">The delegate management operation responses are structured differently than other responses.</span></span> <span data-ttu-id="55d0c-129">As mensagens de resposta do representante gerenciamento são fortemente tipadas.</span><span class="sxs-lookup"><span data-stu-id="55d0c-129">The delegate management response messages are strongly typed.</span></span>
  
<span data-ttu-id="55d0c-130">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server com a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="55d0c-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55d0c-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="55d0c-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55d0c-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="55d0c-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="55d0c-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="55d0c-133">Schema Name</span></span>  <br/> |<span data-ttu-id="55d0c-134">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="55d0c-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="55d0c-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="55d0c-135">Validation File</span></span>  <br/> |<span data-ttu-id="55d0c-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="55d0c-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="55d0c-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="55d0c-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="55d0c-138">False</span><span class="sxs-lookup"><span data-stu-id="55d0c-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55d0c-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="55d0c-139">See also</span></span>



[<span data-ttu-id="55d0c-140">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="55d0c-140">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="55d0c-141">Operação GetDelegate</span><span class="sxs-lookup"><span data-stu-id="55d0c-141">GetDelegate operation</span></span>](getdelegate-operation.md)
  
[<span data-ttu-id="55d0c-142">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="55d0c-142">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
  
[<span data-ttu-id="55d0c-143">Operação RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="55d0c-143">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="55d0c-144">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="55d0c-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

