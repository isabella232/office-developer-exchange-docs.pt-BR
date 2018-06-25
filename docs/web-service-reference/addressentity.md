---
title: AddressEntity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ead22eab-f1e7-48b4-a165-db0e49fe86a8
description: O elemento AddressEntity Especifica a entidade de um único endereço.
ms.openlocfilehash: 6a46a64c9824efdd8df6a08fe1a159e7e42b3731
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751076"
---
# <a name="addressentity"></a><span data-ttu-id="1769f-103">AddressEntity</span><span class="sxs-lookup"><span data-stu-id="1769f-103">AddressEntity</span></span>

<span data-ttu-id="1769f-104">O elemento **AddressEntity** Especifica a entidade de um único endereço.</span><span class="sxs-lookup"><span data-stu-id="1769f-104">The **AddressEntity** element specifies a single address entity.</span></span> 
  
```XML
<AddressEntity>
    <Address></Address>
    <Position></Position>
</AddressEntity>
```

 <span data-ttu-id="1769f-105">**AddressEntityType**</span><span class="sxs-lookup"><span data-stu-id="1769f-105">**AddressEntityType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1769f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1769f-106">Attributes and elements</span></span>

<span data-ttu-id="1769f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1769f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1769f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1769f-108">Attributes</span></span>

<span data-ttu-id="1769f-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1769f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1769f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1769f-110">Child elements</span></span>

|<span data-ttu-id="1769f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1769f-111">**Element**</span></span>|<span data-ttu-id="1769f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1769f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1769f-113">Endereço (string)</span><span class="sxs-lookup"><span data-stu-id="1769f-113">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="1769f-114">Especifica um endereço.</span><span class="sxs-lookup"><span data-stu-id="1769f-114">Specifies an address.</span></span>  <br/> |
|[<span data-ttu-id="1769f-115">Position</span><span class="sxs-lookup"><span data-stu-id="1769f-115">Position</span></span>](position.md) <br/> |<span data-ttu-id="1769f-116">Especifica a posição em uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="1769f-116">Specifies the position in an email message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1769f-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1769f-117">Parent elements</span></span>

|<span data-ttu-id="1769f-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1769f-118">**Element**</span></span>|<span data-ttu-id="1769f-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1769f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1769f-120">Endereços (ArrayOfAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="1769f-120">Addresses (ArrayOfAddressEntitiesType)</span></span>](addresses-arrayofaddressentitiestype.md) <br/> |<span data-ttu-id="1769f-121">Especifica uma matriz de elementos de **AddressEntity** .</span><span class="sxs-lookup"><span data-stu-id="1769f-121">Specifies an array of **AddressEntity** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1769f-122">Text value</span><span class="sxs-lookup"><span data-stu-id="1769f-122">Text value</span></span>

<span data-ttu-id="1769f-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1769f-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1769f-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="1769f-124">Remarks</span></span>

<span data-ttu-id="1769f-125">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1769f-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1769f-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1769f-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1769f-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="1769f-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1769f-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="1769f-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1769f-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1769f-129">Schema Name</span></span>  <br/> |<span data-ttu-id="1769f-130">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="1769f-130">Type schema</span></span>  <br/> |
|<span data-ttu-id="1769f-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1769f-131">Validation File</span></span>  <br/> |<span data-ttu-id="1769f-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1769f-132">types.xsd</span></span>  <br/> |
|<span data-ttu-id="1769f-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="1769f-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1769f-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="1769f-134">See also</span></span>

- [<span data-ttu-id="1769f-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1769f-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

