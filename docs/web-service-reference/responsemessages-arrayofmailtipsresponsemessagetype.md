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
description: O elemento ResponseMessages representa uma lista de mensagens de resposta de dicas de email.
ms.openlocfilehash: 2db58029ead9332b832006bc81d751d77df54b07
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465447"
---
# <a name="responsemessages-arrayofmailtipsresponsemessagetype"></a><span data-ttu-id="cd350-103">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="cd350-103">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>

<span data-ttu-id="cd350-104">O elemento **ResponseMessages** representa uma lista de mensagens de resposta de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="cd350-104">The **ResponseMessages** element represents a list of mail tips response messages.</span></span> 
  
```XML
<ResponseMessages>
   <MailTipsResponseMessageType/>
</ResponseMessages>
```

 <span data-ttu-id="cd350-105">**ArrayOfMailTipsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="cd350-105">**ArrayOfMailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cd350-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="cd350-106">Attributes and elements</span></span>

<span data-ttu-id="cd350-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cd350-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cd350-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cd350-108">Attributes</span></span>

<span data-ttu-id="cd350-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cd350-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cd350-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cd350-110">Child elements</span></span>

|<span data-ttu-id="cd350-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cd350-111">**Element**</span></span>|<span data-ttu-id="cd350-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cd350-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd350-113">MailTipsResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="cd350-113">MailTipsResponseMessageType</span></span>](mailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="cd350-114">Representa configurações de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="cd350-114">Represents mail tips settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cd350-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cd350-115">Parent elements</span></span>

|<span data-ttu-id="cd350-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cd350-116">**Element**</span></span>|<span data-ttu-id="cd350-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cd350-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd350-118">GetMailTipsResponse</span><span class="sxs-lookup"><span data-stu-id="cd350-118">GetMailTipsResponse</span></span>](getmailtipsresponse.md) <br/> |<span data-ttu-id="cd350-119">Representa a mensagem de resposta para a [operação getdicas](getmailtips-operation.md)de email.</span><span class="sxs-lookup"><span data-stu-id="cd350-119">Represents the response message for the [GetMailTips operation](getmailtips-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cd350-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="cd350-120">Text value</span></span>

<span data-ttu-id="cd350-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cd350-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cd350-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="cd350-122">Remarks</span></span>

<span data-ttu-id="cd350-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cd350-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cd350-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="cd350-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cd350-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="cd350-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cd350-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cd350-126">Schema Name</span></span>  <br/> |<span data-ttu-id="cd350-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="cd350-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cd350-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cd350-128">Validation File</span></span>  <br/> |<span data-ttu-id="cd350-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cd350-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cd350-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cd350-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="cd350-131">False</span><span class="sxs-lookup"><span data-stu-id="cd350-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cd350-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="cd350-132">See also</span></span>



[<span data-ttu-id="cd350-133">Operação</span><span class="sxs-lookup"><span data-stu-id="cd350-133">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="cd350-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cd350-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

