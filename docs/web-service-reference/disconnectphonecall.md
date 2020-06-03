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
description: O elemento DisconnectPhoneCall representa uma solicitação para desconectar uma chamada.
ms.openlocfilehash: 8d64ecb9dce1d8b7efcebc70686db8fcbf867217
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529704"
---
# <a name="disconnectphonecall"></a><span data-ttu-id="369e4-103">DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="369e4-103">DisconnectPhoneCall</span></span>

<span data-ttu-id="369e4-104">O elemento **DisconnectPhoneCall** representa uma solicitação para desconectar uma chamada.</span><span class="sxs-lookup"><span data-stu-id="369e4-104">The **DisconnectPhoneCall** element represents a request to disconnect a call.</span></span> 
  
```xml
<DisconnectPhoneCall>
   <PhoneCallId/>
</DisconnectPhoneCall>
```

 <span data-ttu-id="369e4-105">**DisconnectPhoneCallType**</span><span class="sxs-lookup"><span data-stu-id="369e4-105">**DisconnectPhoneCallType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="369e4-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="369e4-106">Attributes and elements</span></span>

<span data-ttu-id="369e4-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="369e4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="369e4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="369e4-108">Attributes</span></span>

<span data-ttu-id="369e4-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="369e4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="369e4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="369e4-110">Child elements</span></span>

|<span data-ttu-id="369e4-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="369e4-111">**Element**</span></span>|<span data-ttu-id="369e4-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="369e4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="369e4-113">Chamada de chamada</span><span class="sxs-lookup"><span data-stu-id="369e4-113">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="369e4-114">Especifica o identificador da chamada a ser desconectada.</span><span class="sxs-lookup"><span data-stu-id="369e4-114">Specifies the identifier of the call to disconnect.</span></span> <span data-ttu-id="369e4-115">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="369e4-115">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="369e4-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="369e4-116">Parent elements</span></span>

<span data-ttu-id="369e4-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="369e4-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="369e4-118">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="369e4-118">Text value</span></span>

<span data-ttu-id="369e4-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="369e4-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="369e4-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="369e4-120">Remarks</span></span>

<span data-ttu-id="369e4-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="369e4-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="369e4-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="369e4-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="369e4-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="369e4-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="369e4-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="369e4-124">Schema Name</span></span>  <br/> |<span data-ttu-id="369e4-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="369e4-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="369e4-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="369e4-126">Validation File</span></span>  <br/> |<span data-ttu-id="369e4-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="369e4-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="369e4-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="369e4-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="369e4-129">False</span><span class="sxs-lookup"><span data-stu-id="369e4-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="369e4-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="369e4-130">See also</span></span>

- [<span data-ttu-id="369e4-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="369e4-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

