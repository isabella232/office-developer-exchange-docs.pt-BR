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
ms.openlocfilehash: 9f11d87ac07dd51a5231d4546fac92e7ca95ad4b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465048"
---
# <a name="updatedelegateresponse"></a><span data-ttu-id="498ef-103">UpdateDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="498ef-103">UpdateDelegateResponse</span></span>

<span data-ttu-id="498ef-104">O elemento **UpdateDelegateResponse** contém o status e o resultado de uma solicitação de [operação UpdateDelegate](updatedelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="498ef-104">The **UpdateDelegateResponse** element contains the status and result of an [UpdateDelegate operation](updatedelegate-operation.md) request.</span></span> 
  
```xml
<UpdateDelegateResponseMessage>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UpdateDelegateResponseMessage>
```

 <span data-ttu-id="498ef-105">**UpdateDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="498ef-105">**UpdateDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="498ef-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="498ef-106">Attributes and elements</span></span>

<span data-ttu-id="498ef-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="498ef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="498ef-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="498ef-108">Attributes</span></span>

<span data-ttu-id="498ef-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="498ef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="498ef-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="498ef-110">Child elements</span></span>

|<span data-ttu-id="498ef-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="498ef-111">**Element**</span></span>|<span data-ttu-id="498ef-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="498ef-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="498ef-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="498ef-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="498ef-114">Contém as mensagens de resposta para uma solicitação de gerenciamento de representante do Exchange Web Services.</span><span class="sxs-lookup"><span data-stu-id="498ef-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="498ef-115">MessageText</span><span class="sxs-lookup"><span data-stu-id="498ef-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="498ef-116">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="498ef-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="498ef-117">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="498ef-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="498ef-118">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="498ef-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="498ef-119">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="498ef-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="498ef-120">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="498ef-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="498ef-121">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="498ef-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="498ef-122">MessageXml</span><span class="sxs-lookup"><span data-stu-id="498ef-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="498ef-123">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="498ef-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="498ef-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="498ef-124">Parent elements</span></span>

<span data-ttu-id="498ef-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="498ef-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="498ef-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="498ef-126">Remarks</span></span>

<span data-ttu-id="498ef-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="498ef-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="498ef-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="498ef-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="498ef-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="498ef-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="498ef-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="498ef-130">Schema Name</span></span>  <br/> |<span data-ttu-id="498ef-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="498ef-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="498ef-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="498ef-132">Validation File</span></span>  <br/> |<span data-ttu-id="498ef-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="498ef-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="498ef-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="498ef-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="498ef-135">False</span><span class="sxs-lookup"><span data-stu-id="498ef-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="498ef-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="498ef-136">See also</span></span>



[<span data-ttu-id="498ef-137">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="498ef-137">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="498ef-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="498ef-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

