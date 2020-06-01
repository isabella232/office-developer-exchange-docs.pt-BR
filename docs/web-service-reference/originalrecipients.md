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
description: O elemento OriginalRecipients representa uma lista de endereços de email dos destinatários da primeira mensagem.
ms.openlocfilehash: 7385b1fd62313ee09c94cd04f3f669215e6cd497
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467176"
---
# <a name="originalrecipients"></a><span data-ttu-id="94062-103">OriginalRecipients</span><span class="sxs-lookup"><span data-stu-id="94062-103">OriginalRecipients</span></span>

<span data-ttu-id="94062-104">O elemento **OriginalRecipients** representa uma lista de endereços de email dos destinatários da primeira mensagem.</span><span class="sxs-lookup"><span data-stu-id="94062-104">The **OriginalRecipients** element represents a list of e-mail addresses of the first message recipients.</span></span> 
  
```XML
<OriginalRecipients>
   <Address/>
</OriginalRecipients>
```

 <span data-ttu-id="94062-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="94062-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94062-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="94062-106">Attributes and elements</span></span>

<span data-ttu-id="94062-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="94062-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94062-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="94062-108">Attributes</span></span>

<span data-ttu-id="94062-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94062-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="94062-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="94062-110">Child elements</span></span>

|<span data-ttu-id="94062-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="94062-111">**Element**</span></span>|<span data-ttu-id="94062-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="94062-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94062-113">Endereço (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="94062-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="94062-114">Contém um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="94062-114">Contains a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="94062-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="94062-115">Parent elements</span></span>

|<span data-ttu-id="94062-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="94062-116">**Element**</span></span>|<span data-ttu-id="94062-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="94062-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94062-118">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="94062-118">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="94062-119">Contém uma única mensagem que é retornada em uma [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="94062-119">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="94062-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="94062-120">Remarks</span></span>

<span data-ttu-id="94062-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="94062-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94062-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="94062-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94062-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="94062-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="94062-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="94062-124">Schema Name</span></span>  <br/> |<span data-ttu-id="94062-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="94062-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="94062-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="94062-126">Validation File</span></span>  <br/> |<span data-ttu-id="94062-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="94062-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="94062-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="94062-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="94062-129">False</span><span class="sxs-lookup"><span data-stu-id="94062-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="94062-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="94062-130">See also</span></span>



[<span data-ttu-id="94062-131">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="94062-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="94062-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="94062-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

