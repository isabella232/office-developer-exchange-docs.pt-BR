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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467176"
---
# <a name="originalrecipients"></a><span data-ttu-id="d81c6-103">OriginalRecipients</span><span class="sxs-lookup"><span data-stu-id="d81c6-103">OriginalRecipients</span></span>

<span data-ttu-id="d81c6-104">O elemento **OriginalRecipients** representa uma lista de endereços de email dos destinatários da primeira mensagem.</span><span class="sxs-lookup"><span data-stu-id="d81c6-104">The **OriginalRecipients** element represents a list of e-mail addresses of the first message recipients.</span></span> 
  
```XML
<OriginalRecipients>
   <Address/>
</OriginalRecipients>
```

 <span data-ttu-id="d81c6-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="d81c6-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d81c6-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d81c6-106">Attributes and elements</span></span>

<span data-ttu-id="d81c6-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d81c6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d81c6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d81c6-108">Attributes</span></span>

<span data-ttu-id="d81c6-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d81c6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d81c6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d81c6-110">Child elements</span></span>

|<span data-ttu-id="d81c6-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d81c6-111">**Element**</span></span>|<span data-ttu-id="d81c6-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d81c6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d81c6-113">Endereço (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="d81c6-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="d81c6-114">Contém um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="d81c6-114">Contains a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d81c6-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d81c6-115">Parent elements</span></span>

|<span data-ttu-id="d81c6-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d81c6-116">**Element**</span></span>|<span data-ttu-id="d81c6-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d81c6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d81c6-118">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="d81c6-118">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="d81c6-119">Contém uma única mensagem que é retornada em uma [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="d81c6-119">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d81c6-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="d81c6-120">Remarks</span></span>

<span data-ttu-id="d81c6-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d81c6-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d81c6-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d81c6-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d81c6-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="d81c6-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d81c6-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d81c6-124">Schema Name</span></span>  <br/> |<span data-ttu-id="d81c6-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d81c6-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="d81c6-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d81c6-126">Validation File</span></span>  <br/> |<span data-ttu-id="d81c6-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d81c6-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d81c6-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d81c6-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="d81c6-129">False</span><span class="sxs-lookup"><span data-stu-id="d81c6-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d81c6-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="d81c6-130">See also</span></span>



[<span data-ttu-id="d81c6-131">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="d81c6-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="d81c6-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d81c6-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

