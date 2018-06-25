---
title: DeliveryRestricted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliveryRestricted
api_type:
- schema
ms.assetid: 05989915-121c-4f26-93cc-af8d454ab442
description: O elemento DeliveryRestricted indica se as restrições de entrega impede que a mensagem do remetente está atingindo o destinatário.
ms.openlocfilehash: ba1c6e00b93c9e442a427fe98a5e15bf5fe1effd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751776"
---
# <a name="deliveryrestricted"></a><span data-ttu-id="4ffd8-103">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="4ffd8-103">DeliveryRestricted</span></span>

<span data-ttu-id="4ffd8-104">O elemento **DeliveryRestricted** indica se as restrições de entrega impede que a mensagem do remetente está atingindo o destinatário.</span><span class="sxs-lookup"><span data-stu-id="4ffd8-104">The **DeliveryRestricted** element indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span> 
  
```XML
<DeliveryRestricted>true | false</DeliveryRestricted>
```

 <span data-ttu-id="4ffd8-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="4ffd8-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ffd8-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4ffd8-106">Attributes and elements</span></span>

<span data-ttu-id="4ffd8-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4ffd8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ffd8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4ffd8-108">Attributes</span></span>

<span data-ttu-id="4ffd8-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4ffd8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ffd8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4ffd8-110">Child elements</span></span>

<span data-ttu-id="4ffd8-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4ffd8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4ffd8-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4ffd8-112">Parent elements</span></span>

|<span data-ttu-id="4ffd8-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4ffd8-113">**Element**</span></span>|<span data-ttu-id="4ffd8-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4ffd8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ffd8-115">Dicas de email</span><span class="sxs-lookup"><span data-stu-id="4ffd8-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="4ffd8-116">Representa os valores para os vários tipos de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="4ffd8-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4ffd8-117">Text value</span><span class="sxs-lookup"><span data-stu-id="4ffd8-117">Text value</span></span>

<span data-ttu-id="4ffd8-118">O valor de texto deste elemento é **true** se as restrições de entrega impedirá que a mensagem do remetente está atingindo o destinatário.</span><span class="sxs-lookup"><span data-stu-id="4ffd8-118">The text value of this element is **true** if delivery restrictions will prevent the sender's message from reaching the recipient.</span></span> <span data-ttu-id="4ffd8-119">O valor é **false** se restrições de entrega não impede que a mensagem do remetente está atingindo o destinatário.</span><span class="sxs-lookup"><span data-stu-id="4ffd8-119">The value is **false** if delivery restrictions will not prevent the sender's message from reaching the recipient.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4ffd8-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="4ffd8-120">Remarks</span></span>

<span data-ttu-id="4ffd8-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ffd8-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ffd8-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4ffd8-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ffd8-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="4ffd8-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4ffd8-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4ffd8-124">Schema Name</span></span>  <br/> |<span data-ttu-id="4ffd8-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4ffd8-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="4ffd8-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4ffd8-126">Validation File</span></span>  <br/> |<span data-ttu-id="4ffd8-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4ffd8-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4ffd8-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4ffd8-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="4ffd8-129">False</span><span class="sxs-lookup"><span data-stu-id="4ffd8-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ffd8-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="4ffd8-130">See also</span></span>

- [<span data-ttu-id="4ffd8-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4ffd8-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

