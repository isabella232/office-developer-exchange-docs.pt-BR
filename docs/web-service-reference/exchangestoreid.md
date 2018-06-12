---
title: ExchangeStoreId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5acceb42-a757-4c74-ab1c-b1abf7bf1e0a
description: O elemento ExchangeStoreId Especifica o identificador de grupo (IM) de mensagens instantâneas.
ms.openlocfilehash: 815e9c2f368558ea38efce3671dbdc33d4d97168
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752129"
---
# <a name="exchangestoreid"></a><span data-ttu-id="4703e-103">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="4703e-103">ExchangeStoreId</span></span>

<span data-ttu-id="4703e-104">O elemento **ExchangeStoreId** Especifica o identificador de grupo (IM) de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="4703e-104">The **ExchangeStoreId** element specifies the instant messaging (IM) group identifier.</span></span> 
  
```XML
<ExchangeStoreId Id="" ChangeKey=""/>
```

 <span data-ttu-id="4703e-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="4703e-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4703e-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4703e-106">Attributes and elements</span></span>

<span data-ttu-id="4703e-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4703e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4703e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4703e-108">Attributes</span></span>

|<span data-ttu-id="4703e-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="4703e-109">**Attribute**</span></span>|<span data-ttu-id="4703e-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4703e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4703e-111">Id</span><span class="sxs-lookup"><span data-stu-id="4703e-111">Id</span></span>  <br/> |<span data-ttu-id="4703e-112">O valor de texto do atributo **Id** é o identificador do grupo.</span><span class="sxs-lookup"><span data-stu-id="4703e-112">The text value of the **Id** attribute is the identifier of the group.</span></span>  <br/> |
|<span data-ttu-id="4703e-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="4703e-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="4703e-114">O valor de texto do atributo **ChangeKey** é a chave de alteração do grupo.</span><span class="sxs-lookup"><span data-stu-id="4703e-114">The text value of the **ChangeKey** attribute is the change key of the group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4703e-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4703e-115">Child elements</span></span>

<span data-ttu-id="4703e-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4703e-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4703e-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4703e-117">Parent elements</span></span>

|<span data-ttu-id="4703e-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4703e-118">**Element**</span></span>|<span data-ttu-id="4703e-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4703e-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4703e-120">ImGroup</span><span class="sxs-lookup"><span data-stu-id="4703e-120">ImGroup</span></span>](imgroup.md) <br/> |<span data-ttu-id="4703e-121">Representa um grupo de mensagens instantâneo.</span><span class="sxs-lookup"><span data-stu-id="4703e-121">Represents an instant messaging group.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4703e-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="4703e-122">Remarks</span></span>

<span data-ttu-id="4703e-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4703e-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4703e-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4703e-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4703e-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4703e-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4703e-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="4703e-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4703e-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4703e-127">Schema Name</span></span>  <br/> |<span data-ttu-id="4703e-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="4703e-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="4703e-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4703e-129">Validation File</span></span>  <br/> |<span data-ttu-id="4703e-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4703e-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4703e-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="4703e-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4703e-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="4703e-132">See also</span></span>



- [<span data-ttu-id="4703e-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4703e-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

