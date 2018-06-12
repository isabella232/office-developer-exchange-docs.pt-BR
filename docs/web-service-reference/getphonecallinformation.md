---
title: GetPhoneCallInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetPhoneCallInformation
api_type:
- schema
ms.assetid: 5f4ee71c-bde0-4b0d-b426-0c24dfe67585
description: O elemento GetPhoneCallInformation Especifica uma solicitação para obter informações sobre a chamada telefônica.
ms.openlocfilehash: 2084a8b5e13b3fa03e0bf62439978bbe81d86ce9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752603"
---
# <a name="getphonecallinformation"></a><span data-ttu-id="3b083-103">GetPhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="3b083-103">GetPhoneCallInformation</span></span>

<span data-ttu-id="3b083-104">O elemento **GetPhoneCallInformation** Especifica uma solicitação para obter informações sobre a chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="3b083-104">The **GetPhoneCallInformation** element specifies a request to get telephone call information.</span></span> 
  
```xml
<GetPhoneCallInformation>
   <PhoneCallId/>
</GetPhoneCallInformation>
```

 <span data-ttu-id="3b083-105">**GetPhoneCallInformationType**</span><span class="sxs-lookup"><span data-stu-id="3b083-105">**GetPhoneCallInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b083-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3b083-106">Attributes and elements</span></span>

<span data-ttu-id="3b083-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3b083-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b083-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3b083-108">Attributes</span></span>

<span data-ttu-id="3b083-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3b083-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b083-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3b083-110">Child elements</span></span>

|<span data-ttu-id="3b083-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3b083-111">**Element**</span></span>|<span data-ttu-id="3b083-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3b083-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b083-113">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="3b083-113">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="3b083-114">Especifica o identificador de uma chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="3b083-114">Specifies the identifier of a phone call.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3b083-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3b083-115">Parent elements</span></span>

<span data-ttu-id="3b083-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3b083-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3b083-117">Text value</span><span class="sxs-lookup"><span data-stu-id="3b083-117">Text value</span></span>

<span data-ttu-id="3b083-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3b083-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3b083-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="3b083-119">Remarks</span></span>

<span data-ttu-id="3b083-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b083-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3b083-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3b083-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b083-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="3b083-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3b083-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3b083-123">Schema Name</span></span>  <br/> |<span data-ttu-id="3b083-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="3b083-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3b083-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3b083-125">Validation File</span></span>  <br/> |<span data-ttu-id="3b083-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3b083-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3b083-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3b083-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="3b083-128">False</span><span class="sxs-lookup"><span data-stu-id="3b083-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3b083-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="3b083-129">See also</span></span>



- [<span data-ttu-id="3b083-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3b083-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

