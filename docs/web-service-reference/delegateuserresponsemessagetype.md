---
title: DelegateUserResponseMessageType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegateUserResponseMessageType
api_type:
- schema
ms.assetid: 3dc9552c-1e2d-40ac-a137-827883c2bb88
description: O elemento DelegateUserResponseMessageType contém a mensagem de resposta para um usuário único representante.
ms.openlocfilehash: ac99e0ca219fc1f1e117f9288d895e27a1df4700
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/21/2018
ms.locfileid: "19751726"
---
# <a name="delegateuserresponsemessagetype"></a><span data-ttu-id="9d3ce-103">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="9d3ce-103">DelegateUserResponseMessageType</span></span>

<span data-ttu-id="9d3ce-104">O elemento **DelegateUserResponseMessageType** contém a mensagem de resposta para um usuário único representante.</span><span class="sxs-lookup"><span data-stu-id="9d3ce-104">The **DelegateUserResponseMessageType** element contains the response message for a single delegate user.</span></span> 
  
```xml
<DelegateUserResponseMessageType>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DelegateUser/>
</DelegateUserResponseMessageType>
```

<span data-ttu-id="9d3ce-105">**DelegateUserResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="9d3ce-105">**DelegateUserResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9d3ce-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9d3ce-106">Attributes and elements</span></span>

<span data-ttu-id="9d3ce-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9d3ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d3ce-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9d3ce-108">Attributes</span></span>

<span data-ttu-id="9d3ce-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9d3ce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d3ce-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9d3ce-110">Child elements</span></span>

|<span data-ttu-id="9d3ce-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9d3ce-111">**Element**</span></span>|<span data-ttu-id="9d3ce-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9d3ce-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d3ce-113">MessageText</span><span class="sxs-lookup"><span data-stu-id="9d3ce-113">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="9d3ce-114">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d3ce-114">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="9d3ce-115">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9d3ce-115">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="9d3ce-116">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d3ce-116">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="9d3ce-117">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9d3ce-117">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="9d3ce-118">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="9d3ce-118">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="9d3ce-119">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="9d3ce-119">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="9d3ce-120">MessageXml</span><span class="sxs-lookup"><span data-stu-id="9d3ce-120">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="9d3ce-121">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="9d3ce-121">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="9d3ce-122">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="9d3ce-122">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="9d3ce-123">Identifica um único representante que é retornado em uma resposta de gerenciamento do representante.</span><span class="sxs-lookup"><span data-stu-id="9d3ce-123">Identifies a single delegate that is returned in a delegate management response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9d3ce-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9d3ce-124">Parent elements</span></span>

|<span data-ttu-id="9d3ce-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9d3ce-125">**Element**</span></span>|<span data-ttu-id="9d3ce-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9d3ce-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d3ce-127">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="9d3ce-127">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="9d3ce-128">Contém as mensagens de resposta para uma solicitação de gerenciamento do representante de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d3ce-128">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9d3ce-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="9d3ce-129">Remarks</span></span>

<span data-ttu-id="9d3ce-130">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server com a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="9d3ce-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d3ce-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9d3ce-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d3ce-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="9d3ce-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9d3ce-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9d3ce-133">Schema Name</span></span>  <br/> |<span data-ttu-id="9d3ce-134">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="9d3ce-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9d3ce-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9d3ce-135">Validation File</span></span>  <br/> |<span data-ttu-id="9d3ce-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9d3ce-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9d3ce-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9d3ce-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d3ce-138">False</span><span class="sxs-lookup"><span data-stu-id="9d3ce-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d3ce-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="9d3ce-139">See also</span></span>

- [<span data-ttu-id="9d3ce-140">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="9d3ce-140">AddDelegate operation</span></span>](adddelegate-operation.md)  
- [<span data-ttu-id="9d3ce-141">Operação GetDelegate</span><span class="sxs-lookup"><span data-stu-id="9d3ce-141">GetDelegate operation</span></span>](getdelegate-operation.md) 
- [<span data-ttu-id="9d3ce-142">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="9d3ce-142">UpdateDelegate operation</span></span>](updatedelegate-operation.md)  
- [<span data-ttu-id="9d3ce-143">Operação RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="9d3ce-143">RemoveDelegate operation</span></span>](removedelegate-operation.md)
- [<span data-ttu-id="9d3ce-144">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9d3ce-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

