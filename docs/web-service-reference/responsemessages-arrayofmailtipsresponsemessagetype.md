---
title: ResponseMessages (ArrayOfMailTipsResponseMessageType)
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
ms.assetid: 00878187-fac2-45b9-ba1c-df7ffac71089
description: O elemento ResponseMessages representa uma lista das mensagens de resposta de dicas de email.
ms.openlocfilehash: 80610af191f3fa600abe2ba8dbba2aac63f3ab1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825192"
---
# <a name="responsemessages-arrayofmailtipsresponsemessagetype"></a><span data-ttu-id="f65cb-103">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="f65cb-103">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>

<span data-ttu-id="f65cb-104">O elemento **ResponseMessages** representa uma lista das mensagens de resposta de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="f65cb-104">The **ResponseMessages** element represents a list of mail tips response messages.</span></span> 
  
```XML
<ResponseMessages>
   <MailTipsResponseMessageType/>
</ResponseMessages>
```

 <span data-ttu-id="f65cb-105">**ArrayOfMailTipsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f65cb-105">**ArrayOfMailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f65cb-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f65cb-106">Attributes and elements</span></span>

<span data-ttu-id="f65cb-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f65cb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f65cb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f65cb-108">Attributes</span></span>

<span data-ttu-id="f65cb-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f65cb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f65cb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f65cb-110">Child elements</span></span>

|<span data-ttu-id="f65cb-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f65cb-111">**Element**</span></span>|<span data-ttu-id="f65cb-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f65cb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f65cb-113">MailTipsResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="f65cb-113">MailTipsResponseMessageType</span></span>](mailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="f65cb-114">Representa as configurações de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="f65cb-114">Represents mail tips settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f65cb-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f65cb-115">Parent elements</span></span>

|<span data-ttu-id="f65cb-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f65cb-116">**Element**</span></span>|<span data-ttu-id="f65cb-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f65cb-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f65cb-118">GetMailTipsResponse</span><span class="sxs-lookup"><span data-stu-id="f65cb-118">GetMailTipsResponse</span></span>](getmailtipsresponse.md) <br/> |<span data-ttu-id="f65cb-119">Representa a mensagem de resposta para a [operação GetMailTips](getmailtips-operation.md).</span><span class="sxs-lookup"><span data-stu-id="f65cb-119">Represents the response message for the [GetMailTips operation](getmailtips-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f65cb-120">Text value</span><span class="sxs-lookup"><span data-stu-id="f65cb-120">Text value</span></span>

<span data-ttu-id="f65cb-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f65cb-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f65cb-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="f65cb-122">Remarks</span></span>

<span data-ttu-id="f65cb-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f65cb-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f65cb-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f65cb-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f65cb-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="f65cb-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f65cb-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f65cb-126">Schema Name</span></span>  <br/> |<span data-ttu-id="f65cb-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="f65cb-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f65cb-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f65cb-128">Validation File</span></span>  <br/> |<span data-ttu-id="f65cb-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f65cb-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f65cb-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f65cb-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="f65cb-131">False</span><span class="sxs-lookup"><span data-stu-id="f65cb-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f65cb-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="f65cb-132">See also</span></span>



[<span data-ttu-id="f65cb-133">Operação GetMailTips</span><span class="sxs-lookup"><span data-stu-id="f65cb-133">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="f65cb-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f65cb-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

