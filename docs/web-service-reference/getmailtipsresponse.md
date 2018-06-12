---
title: GetMailTipsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTipsResponse
api_type:
- schema
ms.assetid: fe270e34-566e-4f9e-9e73-fbf38e06436d
description: O elemento GetMailTipsResponse representa a mensagem de resposta para uma operação de GetMailTips.
ms.openlocfilehash: e7a18e8818761af931d32b26aeaf58a2853fa684
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752555"
---
# <a name="getmailtipsresponse"></a><span data-ttu-id="2c381-103">GetMailTipsResponse</span><span class="sxs-lookup"><span data-stu-id="2c381-103">GetMailTipsResponse</span></span>

<span data-ttu-id="2c381-104">O elemento **GetMailTipsResponse** representa a mensagem de resposta para uma [operação de GetMailTips](getmailtips-operation.md).</span><span class="sxs-lookup"><span data-stu-id="2c381-104">The **GetMailTipsResponse** element represents the response message for a [GetMailTips operation](getmailtips-operation.md).</span></span>
  
```XML
<GetMailTipsResponse>
   <ResponseMessages/>
</GetMailTipsResponse>
```

 <span data-ttu-id="2c381-105">**GetMailTipsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="2c381-105">**GetMailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2c381-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2c381-106">Attributes and elements</span></span>

<span data-ttu-id="2c381-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2c381-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2c381-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2c381-108">Attributes</span></span>

<span data-ttu-id="2c381-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2c381-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2c381-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2c381-110">Child elements</span></span>

|<span data-ttu-id="2c381-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2c381-111">**Element**</span></span>|<span data-ttu-id="2c381-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2c381-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c381-113">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="2c381-113">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>](responsemessages-arrayofmailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="2c381-114">Representa uma lista das mensagens de resposta de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="2c381-114">Represents a list of mail tips response messages.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2c381-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2c381-115">Parent elements</span></span>

<span data-ttu-id="2c381-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2c381-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="2c381-117">Text value</span><span class="sxs-lookup"><span data-stu-id="2c381-117">Text value</span></span>

<span data-ttu-id="2c381-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2c381-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2c381-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="2c381-119">Remarks</span></span>

<span data-ttu-id="2c381-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2c381-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2c381-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2c381-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2c381-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="2c381-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2c381-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2c381-123">Schema Name</span></span>  <br/> |<span data-ttu-id="2c381-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="2c381-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2c381-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2c381-125">Validation File</span></span>  <br/> |<span data-ttu-id="2c381-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2c381-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2c381-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2c381-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="2c381-128">False</span><span class="sxs-lookup"><span data-stu-id="2c381-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2c381-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="2c381-129">See also</span></span>



[<span data-ttu-id="2c381-130">Operação GetMailTips</span><span class="sxs-lookup"><span data-stu-id="2c381-130">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="2c381-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2c381-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

