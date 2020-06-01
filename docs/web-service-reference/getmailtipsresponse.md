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
description: O elemento GetMailTipsResponse representa a mensagem de resposta para uma operação condicas de email.
ms.openlocfilehash: 2c0dcfe4e2deddcf9a6f4bb9d68d59115c171796
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458604"
---
# <a name="getmailtipsresponse"></a><span data-ttu-id="ff8bf-103">GetMailTipsResponse</span><span class="sxs-lookup"><span data-stu-id="ff8bf-103">GetMailTipsResponse</span></span>

<span data-ttu-id="ff8bf-104">O elemento **GetMailTipsResponse** representa a mensagem de resposta para uma [operação condicas](getmailtips-operation.md)de email.</span><span class="sxs-lookup"><span data-stu-id="ff8bf-104">The **GetMailTipsResponse** element represents the response message for a [GetMailTips operation](getmailtips-operation.md).</span></span>
  
```XML
<GetMailTipsResponse>
   <ResponseMessages/>
</GetMailTipsResponse>
```

 <span data-ttu-id="ff8bf-105">**GetMailTipsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="ff8bf-105">**GetMailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff8bf-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ff8bf-106">Attributes and elements</span></span>

<span data-ttu-id="ff8bf-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ff8bf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff8bf-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ff8bf-108">Attributes</span></span>

<span data-ttu-id="ff8bf-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff8bf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff8bf-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ff8bf-110">Child elements</span></span>

|<span data-ttu-id="ff8bf-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ff8bf-111">**Element**</span></span>|<span data-ttu-id="ff8bf-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ff8bf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff8bf-113">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="ff8bf-113">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>](responsemessages-arrayofmailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="ff8bf-114">Representa uma lista de mensagens de resposta de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="ff8bf-114">Represents a list of mail tips response messages.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ff8bf-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ff8bf-115">Parent elements</span></span>

<span data-ttu-id="ff8bf-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff8bf-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="ff8bf-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="ff8bf-117">Text value</span></span>

<span data-ttu-id="ff8bf-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ff8bf-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ff8bf-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="ff8bf-119">Remarks</span></span>

<span data-ttu-id="ff8bf-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff8bf-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff8bf-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ff8bf-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff8bf-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="ff8bf-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ff8bf-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ff8bf-123">Schema Name</span></span>  <br/> |<span data-ttu-id="ff8bf-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ff8bf-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ff8bf-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ff8bf-125">Validation File</span></span>  <br/> |<span data-ttu-id="ff8bf-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ff8bf-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ff8bf-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ff8bf-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="ff8bf-128">False</span><span class="sxs-lookup"><span data-stu-id="ff8bf-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ff8bf-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="ff8bf-129">See also</span></span>



[<span data-ttu-id="ff8bf-130">Operação</span><span class="sxs-lookup"><span data-stu-id="ff8bf-130">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="ff8bf-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ff8bf-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

