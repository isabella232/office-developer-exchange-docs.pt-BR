---
title: UpdateDelegateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateDelegateResponse
api_type:
- schema
ms.assetid: cd336add-fbcc-4f61-9867-d4c08a60e142
description: O elemento UpdateDelegateResponse contém o status e o resultado de uma solicitação de operação UpdateDelegate.
ms.openlocfilehash: b90dd7d8011cf75831481b8f2b92df80d9a67d31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837870"
---
# <a name="updatedelegateresponse"></a><span data-ttu-id="19a4a-103">UpdateDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="19a4a-103">UpdateDelegateResponse</span></span>

<span data-ttu-id="19a4a-104">O elemento **UpdateDelegateResponse** contém o status e o resultado de uma solicitação de [operação UpdateDelegate](updatedelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="19a4a-104">The **UpdateDelegateResponse** element contains the status and result of an [UpdateDelegate operation](updatedelegate-operation.md) request.</span></span> 
  
```xml
<UpdateDelegateResponseMessage>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UpdateDelegateResponseMessage>
```

 <span data-ttu-id="19a4a-105">**UpdateDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="19a4a-105">**UpdateDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19a4a-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="19a4a-106">Attributes and elements</span></span>

<span data-ttu-id="19a4a-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="19a4a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19a4a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="19a4a-108">Attributes</span></span>

<span data-ttu-id="19a4a-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="19a4a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19a4a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="19a4a-110">Child elements</span></span>

|<span data-ttu-id="19a4a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="19a4a-111">**Element**</span></span>|<span data-ttu-id="19a4a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="19a4a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19a4a-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="19a4a-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="19a4a-114">Contém as mensagens de resposta para uma solicitação de gerenciamento do representante de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="19a4a-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="19a4a-115">MessageText</span><span class="sxs-lookup"><span data-stu-id="19a4a-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="19a4a-116">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="19a4a-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="19a4a-117">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="19a4a-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="19a4a-118">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="19a4a-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="19a4a-119">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="19a4a-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="19a4a-120">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="19a4a-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="19a4a-121">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="19a4a-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="19a4a-122">MessageXml</span><span class="sxs-lookup"><span data-stu-id="19a4a-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="19a4a-123">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="19a4a-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="19a4a-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="19a4a-124">Parent elements</span></span>

<span data-ttu-id="19a4a-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="19a4a-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="19a4a-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="19a4a-126">Remarks</span></span>

<span data-ttu-id="19a4a-127">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="19a4a-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19a4a-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="19a4a-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19a4a-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="19a4a-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="19a4a-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="19a4a-130">Schema Name</span></span>  <br/> |<span data-ttu-id="19a4a-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="19a4a-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="19a4a-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="19a4a-132">Validation File</span></span>  <br/> |<span data-ttu-id="19a4a-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="19a4a-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="19a4a-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="19a4a-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="19a4a-135">False</span><span class="sxs-lookup"><span data-stu-id="19a4a-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="19a4a-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="19a4a-136">See also</span></span>



[<span data-ttu-id="19a4a-137">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="19a4a-137">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="19a4a-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="19a4a-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

