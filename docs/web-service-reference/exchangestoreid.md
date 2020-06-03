---
title: ExchangeStoreId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5acceb42-a757-4c74-ab1c-b1abf7bf1e0a
description: O elemento ExchangeStoreId especifica o identificador de grupo de mensagens instantâneas (IM).
ms.openlocfilehash: c1b1e1830987449eeb7ea186d00743ea9cc75a77
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456987"
---
# <a name="exchangestoreid"></a><span data-ttu-id="441b2-103">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="441b2-103">ExchangeStoreId</span></span>

<span data-ttu-id="441b2-104">O elemento **ExchangeStoreId** especifica o identificador de grupo de mensagens instantâneas (IM).</span><span class="sxs-lookup"><span data-stu-id="441b2-104">The **ExchangeStoreId** element specifies the instant messaging (IM) group identifier.</span></span> 
  
```XML
<ExchangeStoreId Id="" ChangeKey=""/>
```

 <span data-ttu-id="441b2-105">**ItemIdtype**</span><span class="sxs-lookup"><span data-stu-id="441b2-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="441b2-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="441b2-106">Attributes and elements</span></span>

<span data-ttu-id="441b2-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="441b2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="441b2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="441b2-108">Attributes</span></span>

|<span data-ttu-id="441b2-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="441b2-109">**Attribute**</span></span>|<span data-ttu-id="441b2-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="441b2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="441b2-111">Id</span><span class="sxs-lookup"><span data-stu-id="441b2-111">Id</span></span>  <br/> |<span data-ttu-id="441b2-112">O valor de texto do atributo **ID** é o identificador do grupo.</span><span class="sxs-lookup"><span data-stu-id="441b2-112">The text value of the **Id** attribute is the identifier of the group.</span></span>  <br/> |
|<span data-ttu-id="441b2-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="441b2-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="441b2-114">O valor de texto do atributo **ChangeKey** é a chave de alteração do grupo.</span><span class="sxs-lookup"><span data-stu-id="441b2-114">The text value of the **ChangeKey** attribute is the change key of the group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="441b2-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="441b2-115">Child elements</span></span>

<span data-ttu-id="441b2-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="441b2-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="441b2-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="441b2-117">Parent elements</span></span>

|<span data-ttu-id="441b2-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="441b2-118">**Element**</span></span>|<span data-ttu-id="441b2-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="441b2-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="441b2-120">Imgroup</span><span class="sxs-lookup"><span data-stu-id="441b2-120">ImGroup</span></span>](imgroup.md) <br/> |<span data-ttu-id="441b2-121">Representa um grupo de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="441b2-121">Represents an instant messaging group.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="441b2-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="441b2-122">Remarks</span></span>

<span data-ttu-id="441b2-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="441b2-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="441b2-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="441b2-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="441b2-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="441b2-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="441b2-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="441b2-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="441b2-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="441b2-127">Schema Name</span></span>  <br/> |<span data-ttu-id="441b2-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="441b2-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="441b2-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="441b2-129">Validation File</span></span>  <br/> |<span data-ttu-id="441b2-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="441b2-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="441b2-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="441b2-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="441b2-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="441b2-132">See also</span></span>



- [<span data-ttu-id="441b2-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="441b2-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

