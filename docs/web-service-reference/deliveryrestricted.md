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
description: O elemento DeliveryRestricted indica se as restrições de entrega impedirão que a mensagem do remetente atinja o destinatário.
ms.openlocfilehash: 58fc85873326179d7745db4ba7d4854a76ced6a7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462686"
---
# <a name="deliveryrestricted"></a><span data-ttu-id="ffad2-103">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="ffad2-103">DeliveryRestricted</span></span>

<span data-ttu-id="ffad2-104">O elemento **DeliveryRestricted** indica se as restrições de entrega impedirão que a mensagem do remetente atinja o destinatário.</span><span class="sxs-lookup"><span data-stu-id="ffad2-104">The **DeliveryRestricted** element indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span> 
  
```XML
<DeliveryRestricted>true | false</DeliveryRestricted>
```

 <span data-ttu-id="ffad2-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="ffad2-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ffad2-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ffad2-106">Attributes and elements</span></span>

<span data-ttu-id="ffad2-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ffad2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ffad2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ffad2-108">Attributes</span></span>

<span data-ttu-id="ffad2-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ffad2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ffad2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ffad2-110">Child elements</span></span>

<span data-ttu-id="ffad2-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ffad2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ffad2-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ffad2-112">Parent elements</span></span>

|<span data-ttu-id="ffad2-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ffad2-113">**Element**</span></span>|<span data-ttu-id="ffad2-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ffad2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ffad2-115">Dicas de Email</span><span class="sxs-lookup"><span data-stu-id="ffad2-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="ffad2-116">Representa valores de vários tipos de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="ffad2-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ffad2-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="ffad2-117">Text value</span></span>

<span data-ttu-id="ffad2-118">O valor de texto desse elemento será **true** se as restrições de entrega impedirão que a mensagem do remetente atinja o destinatário.</span><span class="sxs-lookup"><span data-stu-id="ffad2-118">The text value of this element is **true** if delivery restrictions will prevent the sender's message from reaching the recipient.</span></span> <span data-ttu-id="ffad2-119">O valor é **false** se as restrições de entrega não impedem que a mensagem do remetente atinja o destinatário.</span><span class="sxs-lookup"><span data-stu-id="ffad2-119">The value is **false** if delivery restrictions will not prevent the sender's message from reaching the recipient.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ffad2-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="ffad2-120">Remarks</span></span>

<span data-ttu-id="ffad2-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ffad2-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ffad2-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ffad2-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ffad2-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="ffad2-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ffad2-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ffad2-124">Schema Name</span></span>  <br/> |<span data-ttu-id="ffad2-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ffad2-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="ffad2-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ffad2-126">Validation File</span></span>  <br/> |<span data-ttu-id="ffad2-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ffad2-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ffad2-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ffad2-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="ffad2-129">False</span><span class="sxs-lookup"><span data-stu-id="ffad2-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ffad2-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="ffad2-130">See also</span></span>

- [<span data-ttu-id="ffad2-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ffad2-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

