---
title: InvalidRecipient (dicas de email)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InvalidRecipient
api_type:
- schema
ms.assetid: 48959a99-bb0d-4004-963e-5a5baaa96476
description: O elemento InvalidRecipient indica se o destinatário é inválido.
ms.openlocfilehash: addb86ece2be3091ac55a52ee2f16f5c5f72ae41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823958"
---
# <a name="invalidrecipient-mailtips"></a><span data-ttu-id="1c145-103">InvalidRecipient (dicas de email)</span><span class="sxs-lookup"><span data-stu-id="1c145-103">InvalidRecipient (MailTips)</span></span>

<span data-ttu-id="1c145-104">O elemento **InvalidRecipient** indica se o destinatário é inválido.</span><span class="sxs-lookup"><span data-stu-id="1c145-104">The **InvalidRecipient** element indicates whether the recipient is invalid.</span></span> 
  
```XML
<InvalidRecipient>true | false</InvalidRecipient>
```

 <span data-ttu-id="1c145-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="1c145-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1c145-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1c145-106">Attributes and elements</span></span>

<span data-ttu-id="1c145-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1c145-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1c145-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1c145-108">Attributes</span></span>

<span data-ttu-id="1c145-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1c145-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1c145-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1c145-110">Child elements</span></span>

<span data-ttu-id="1c145-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1c145-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1c145-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1c145-112">Parent elements</span></span>

|<span data-ttu-id="1c145-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1c145-113">**Element**</span></span>|<span data-ttu-id="1c145-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1c145-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c145-115">Dicas de email</span><span class="sxs-lookup"><span data-stu-id="1c145-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="1c145-116">Representa os valores para os vários tipos de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="1c145-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1c145-117">Text value</span><span class="sxs-lookup"><span data-stu-id="1c145-117">Text value</span></span>

<span data-ttu-id="1c145-118">O valor de texto deste elemento é **true** se o destinatário é inválido.</span><span class="sxs-lookup"><span data-stu-id="1c145-118">The text value of this element is **true** if the recipient is invalid.</span></span> <span data-ttu-id="1c145-119">O valor é **false** se o destinatário não é inválido.</span><span class="sxs-lookup"><span data-stu-id="1c145-119">The value is **false** if the recipient is not invalid.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1c145-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="1c145-120">Remarks</span></span>

<span data-ttu-id="1c145-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1c145-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1c145-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="1c145-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1c145-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="1c145-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1c145-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1c145-124">Schema Name</span></span>  <br/> |<span data-ttu-id="1c145-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="1c145-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="1c145-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1c145-126">Validation File</span></span>  <br/> |<span data-ttu-id="1c145-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1c145-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1c145-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1c145-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="1c145-129">False</span><span class="sxs-lookup"><span data-stu-id="1c145-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1c145-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="1c145-130">See also</span></span>



- [<span data-ttu-id="1c145-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1c145-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

