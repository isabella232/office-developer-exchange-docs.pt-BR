---
title: OriginalRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OriginalRecipients
api_type:
- schema
ms.assetid: e4af86a5-85af-4239-8055-e29f0acf77c1
description: O elemento OriginalRecipients representa uma lista de endereços de email dos destinatários da mensagem primeiro.
ms.openlocfilehash: 8f99368409dbfb5ac798b691be65c7fd64f32660
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824665"
---
# <a name="originalrecipients"></a><span data-ttu-id="e5207-103">OriginalRecipients</span><span class="sxs-lookup"><span data-stu-id="e5207-103">OriginalRecipients</span></span>

<span data-ttu-id="e5207-104">O elemento **OriginalRecipients** representa uma lista de endereços de email dos destinatários da mensagem primeiro.</span><span class="sxs-lookup"><span data-stu-id="e5207-104">The **OriginalRecipients** element represents a list of e-mail addresses of the first message recipients.</span></span> 
  
```XML
<OriginalRecipients>
   <Address/>
</OriginalRecipients>
```

 <span data-ttu-id="e5207-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="e5207-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e5207-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e5207-106">Attributes and elements</span></span>

<span data-ttu-id="e5207-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e5207-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e5207-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e5207-108">Attributes</span></span>

<span data-ttu-id="e5207-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e5207-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e5207-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e5207-110">Child elements</span></span>

|<span data-ttu-id="e5207-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e5207-111">**Element**</span></span>|<span data-ttu-id="e5207-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e5207-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5207-113">Endereço (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="e5207-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="e5207-114">Contém um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="e5207-114">Contains a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e5207-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e5207-115">Parent elements</span></span>

|<span data-ttu-id="e5207-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e5207-116">**Element**</span></span>|<span data-ttu-id="e5207-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e5207-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5207-118">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="e5207-118">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="e5207-119">Contém uma única mensagem retornada em uma [operação de GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="e5207-119">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e5207-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="e5207-120">Remarks</span></span>

<span data-ttu-id="e5207-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e5207-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e5207-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e5207-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e5207-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="e5207-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e5207-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e5207-124">Schema Name</span></span>  <br/> |<span data-ttu-id="e5207-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e5207-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="e5207-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e5207-126">Validation File</span></span>  <br/> |<span data-ttu-id="e5207-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e5207-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e5207-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e5207-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="e5207-129">False</span><span class="sxs-lookup"><span data-stu-id="e5207-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e5207-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="e5207-130">See also</span></span>



[<span data-ttu-id="e5207-131">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="e5207-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="e5207-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e5207-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

