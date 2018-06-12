---
title: DisconnectPhoneCall
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DisconnectPhoneCall
api_type:
- schema
ms.assetid: f9252536-9852-4dd9-9ebc-91f5cf281171
description: O elemento DisconnectPhoneCall representa uma solicitação para desconectar chamada.
ms.openlocfilehash: 56947ea9ba56c76bb02d6a425ff43b3b846a2f60
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751847"
---
# <a name="disconnectphonecall"></a><span data-ttu-id="6165c-103">DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="6165c-103">DisconnectPhoneCall</span></span>

<span data-ttu-id="6165c-104">O elemento **DisconnectPhoneCall** representa uma solicitação para desconectar chamada.</span><span class="sxs-lookup"><span data-stu-id="6165c-104">The **DisconnectPhoneCall** element represents a request to disconnect a call.</span></span> 
  
```xml
<DisconnectPhoneCall>
   <PhoneCallId/>
</DisconnectPhoneCall>
```

 <span data-ttu-id="6165c-105">**DisconnectPhoneCallType**</span><span class="sxs-lookup"><span data-stu-id="6165c-105">**DisconnectPhoneCallType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6165c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6165c-106">Attributes and elements</span></span>

<span data-ttu-id="6165c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6165c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6165c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6165c-108">Attributes</span></span>

<span data-ttu-id="6165c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6165c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6165c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6165c-110">Child elements</span></span>

|<span data-ttu-id="6165c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6165c-111">**Element**</span></span>|<span data-ttu-id="6165c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6165c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6165c-113">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="6165c-113">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="6165c-114">Especifica o identificador da chamada ser desconectada.</span><span class="sxs-lookup"><span data-stu-id="6165c-114">Specifies the identifier of the call to disconnect.</span></span> <span data-ttu-id="6165c-115">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6165c-115">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6165c-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6165c-116">Parent elements</span></span>

<span data-ttu-id="6165c-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6165c-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="6165c-118">Text value</span><span class="sxs-lookup"><span data-stu-id="6165c-118">Text value</span></span>

<span data-ttu-id="6165c-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6165c-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6165c-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="6165c-120">Remarks</span></span>

<span data-ttu-id="6165c-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6165c-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6165c-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6165c-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6165c-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="6165c-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6165c-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6165c-124">Schema Name</span></span>  <br/> |<span data-ttu-id="6165c-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="6165c-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6165c-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6165c-126">Validation File</span></span>  <br/> |<span data-ttu-id="6165c-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6165c-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6165c-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6165c-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="6165c-129">False</span><span class="sxs-lookup"><span data-stu-id="6165c-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6165c-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="6165c-130">See also</span></span>

- [<span data-ttu-id="6165c-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6165c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

